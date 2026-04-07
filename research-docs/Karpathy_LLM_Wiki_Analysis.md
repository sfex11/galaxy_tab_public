# Karpathy의 LLM Wiki 패턴 분석 및 OpenClaw 도입 제안

**분석일**: 2026-04-05  
**출처**: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f

---

## 📋 개요

Karpathy가 제안한 **LLM Wiki 패턴**은 RAG의 한계를 극복하고 지식을 지속적으로 축적하는 새로운 접근법입니다.

---

## 🔑 핵심 아이디어

### RAG vs LLM Wiki

| RAG | LLM Wiki |
|-----|----------|
| 매번 원본에서 검색 | 지식이 미리 컴파일됨 |
| 재발견 반복 | 축적 및 진화 |
| 쿼리 시간에 조립 | 교차 참조 미리 구축 |
| 모순 처리 안 됨 | 모순 자동 플래깅 |

**핵심 차이점**: Wiki는 **지속 가능한(compounding) 아티팩트**입니다.

---

## 🏗️ 3계층 아키텍처

### 1. Raw Sources (원본)
- 특성: **불변(immutable)**
- 내용: 논문, 기사, 이미지, 데이터 파일
- 역할: Source of Truth
- OpenClaw 적용: `/storage/B8AC-56F1/papers/*.json`

### 2. Wiki (지식 기반)
- 특성: **LLM이 소유 및 관리**
- 내용: 요약, 엔티티 페이지, 개념 페이지, 비교, 개요, 종합
- 역할: 지속 진화하는 지식 베이스
- OpenClaw 적용: `~/.openclaw/workspace/wiki/` (신규 생성 필요)

### 3. Schema (설정)
- 특성: **LLM과 공동 진화**
- 내용: Wiki 구조, 규칙, 워크플로우
- 역할: LLM을 규율된 wiki 관리자로 만듦
- OpenClaw 적용: `WIKI_SCHEMA.md` (신규 생성 필요)

---

## 🔄 워크플로우

### 1. Ingest (섭취)

**프로세스**:
1. 새 소스를 raw collection에 추가
2. LLM이 소스 읽기
3. 사용자와 핵심 내용 논의
4. Wiki에 요약 페이지 작성
5. Index 업데이트
6. 관련 엔티티/개념 페이지 업데이트
7. Log에 항목 추가

**하나의 소스 → 10-15개 wiki 페이지 터치**

**OpenClaw 적용**:
```python
# 논문 수집 시 자동으로 wiki 업데이트
def ingest_paper(paper_id):
    # 1. 논문 수집 (기존)
    paper = collect_paper(paper_id)
    
    # 2. Wiki 업데이트 (신규)
    update_wiki(paper)
    
def update_wiki(paper):
    # 요약 페이지 생성
    create_summary_page(paper)
    
    # 엔티티 페이지 업데이트
    # 예: "LLM Agent", "Reinforcement Learning"
    update_entity_pages(paper)
    
    # 개념 페이지 업데이트
    # 예: "Emotion Vector", "Activation Steering"
    update_concept_pages(paper)
    
    # Index 업데이트
    update_index(paper)
    
    # Log 추가
    append_log(f"ingest | {paper['title']}")
```

### 2. Query (질의)

**프로세스**:
1. Wiki에서 관련 페이지 검색
2. 페이지 읽기 및 종합
3. 인용과 함께 답변 생성
4. **중요**: 좋은 답변은 다시 wiki에 파일링

**OpenClaw 적용**:
```python
def query_wiki(question):
    # 1. Index에서 관련 페이지 찾기
    relevant_pages = search_index(question)
    
    # 2. 페이지 읽기
    context = read_pages(relevant_pages)
    
    # 3. 답변 생성
    answer = synthesize_answer(question, context)
    
    # 4. 좋은 답변은 wiki에 저장
    if is_valuable(answer):
        create_wiki_page(answer, type="query_result")
    
    return answer
```

### 3. Lint (건전성 체크)

**주기적으로 수행**:
- 페이지 간 모순 검사
- 오래된 주장 식별
- 고아 페이지(orphan pages) 찾기
- 누락된 교차 참조
- 데이터 갭 식별

**OpenClaw 적용**:
```python
def lint_wiki():
    issues = []
    
    # 1. 모순 검사
    contradictions = find_contradictions()
    issues.extend(contradictions)
    
    # 2. 고아 페이지
    orphans = find_orphan_pages()
    issues.extend(orphans)
    
    # 3. 누락된 참조
    missing_refs = find_missing_references()
    issues.extend(missing_refs)
    
    # 4. 개선 제안
    suggestions = suggest_improvements()
    
    return {
        "issues": issues,
        "suggestions": suggestions
    }
```

---

## 📄 특수 파일

### 1. index.md (콘텐츠 카탈로그)

**용도**: Wiki의 모든 페이지 목록

**구조**:
```markdown
# Wiki Index

## Entities
- [[LLM Agent]] - 자율 에이전트 관련 연구
- [[Emotion Vector]] - 감정 표현 벡터 연구

## Concepts
- [[Activation Steering]] - 활성화 조향 기법
- [[Representation Engineering]] - 표현 엔지니어링

## Sources
- [[2026-04-03-ActionParty]] - 다중 에이전트 제어 (2026-04-03)
- [[2026-04-04-Steerable]] - 조향 가능한 시각 표현 (2026-04-04)

## Query Results
- [[Emotion vs Behavior Comparison]] - 감정-행동 비교 분석
```

**OpenClaw 적용**:
```python
def update_index(new_page):
    """모든 ingest 시 index.md 업데이트"""
    with open('wiki/index.md', 'a') as f:
        category = classify_page(new_page)
        entry = f"- [[{new_page.title}]] - {new_page.summary}\n"
        f.write(f"## {category}\n{entry}")
```

### 2. log.md (작업 타임라인)

**용도**: Wiki 진화 기록

**구조**:
```markdown
# Wiki Log

## [2026-04-03] ingest | ActionParty: Multi-Subject Action Binding
- 요약 페이지 생성
- LLM Agent 엔티티 업데이트
- Multi-Agent System 개념 추가

## [2026-04-03] query | "감정 벡터와 행동의 관계는?"
- Emotion Vector 페이지 읽기
- Behavior 페이지 읽기
- 비교 분석 페이지 생성

## [2026-04-04] lint | 전체 wiki 건전성 체크
- 3개 모순 발견
- 5개 고아 페이지 식별
- 2개 참조 누락
```

**파싱 가능**:
```bash
grep "^## \[" log.md | tail -5  # 최근 5개 항목
```

**OpenClaw 적용**:
```python
def append_log(action, details):
    """모든 작업을 log.md에 기록"""
    timestamp = datetime.now().strftime('%Y-%m-%d %H:%M')
    entry = f"## [{timestamp}] {action} | {details}\n"
    
    with open('wiki/log.md', 'a') as f:
        f.write(entry)
```

---

## 🛠️ 도구

### 1. qmd (Markdown 검색 엔진)

**기능**:
- Hybrid BM25/vector search
- LLM re-ranking
- CLI + MCP server

**OpenClaw 도입 가치**: ⭐⭐⭐⭐⭐ (매우 높음)

**이유**:
- 현재 64개 요약 + 68개 슬라이드 → 검색 필요
- Wiki가 커질수록 index.md만으로는 부족
- LLM이 쉘 아웃으로 사용 가능

**설치**:
```bash
pip install qmd
# 또는
git clone https://github.com/tobi/qmd
```

**사용**:
```python
def search_wiki(query):
    """qmd로 wiki 검색"""
    result = subprocess.run(
        ['qmd', 'search', query, '--path', 'wiki/'],
        capture_output=True,
        text=True
    )
    return parse_results(result.stdout)
```

### 2. Obsidian Web Clipper

**기능**: 웹 기사 → 마크다운 변환

**OpenClaw 도입 가치**: ⭐⭐⭐ (보통)

**이유**:
- 현재 paper-collector가 arXiv 처리
- 일반 웹 기사도 수집하려면 유용
- 하지만 당장은 논문 중심이므로 우선순위 낮음

### 3. 이미지 다운로드

**기능**: 로컬 이미지 다운로드

**OpenClaw 도입 가치**: ⭐⭐ (낮음)

**이유**:
- 현재 텍스트 위주
- 이미지 처리는 나중에 고려

### 4. Marp (슬라이드)

**기능**: Markdown → 슬라이드

**OpenClaw 도입 가치**: ⭐⭐⭐⭐⭐ (매우 높음)

**이유**:
- 이미 68개 HTML 슬라이드 존재
- Marp로 통일하면 관리 용이
- Wiki에서 바로 슬라이드 생성 가능

**전환 방안**:
```python
def create_marp_slides(wiki_page):
    """Wiki 페이지 → Marp 슬라이드"""
    slides = f"""
---
marp: true
---

# {wiki_page.title}

{wiki_page.summary}

---

## 인사이트

{wiki_page.insights}

---

## 응용

{wiki_page.applications}
"""
    return slides
```

### 5. Dataview (쿼리)

**기능**: YAML frontmatter 기반 쿼리

**OpenClaw 도입 가치**: ⭐⭐⭐ (보통)

**이유**:
- Wiki에 YAML 메타데이터 추가하면 유용
- 동적 테이블 생성 가능
- 하지만 필수는 아님

**예시**:
```markdown
---
tags: [emotion, llm, steering]
date: 2026-04-03
sources: 5
---

# Emotion Vector

```dataview
TABLE date, sources
FROM #emotion
SORT date DESC
```
```

---

## 🚀 OpenClaw 도입 계획

### Phase 1: Wiki 구조 설계 (1주)

**1.1 디렉토리 생성**
```
~/.openclaw/workspace/wiki/
├── index.md
├── log.md
├── entities/
│   ├── llm-agent.md
│   ├── emotion-vector.md
│   └── ...
├── concepts/
│   ├── activation-steering.md
│   ├── representation-engineering.md
│   └── ...
├── sources/
│   ├── 2026-04-03-ActionParty.md
│   ├── 2026-04-04-Steerable.md
│   └── ...
├── queries/
│   ├── emotion-behavior-comparison.md
│   └── ...
└── WIKI_SCHEMA.md
```

**1.2 Schema 작성**

`WIKI_SCHEMA.md`:
```markdown
# Wiki Schema

## 구조

### Entities (엔티티)
- 연구 대상 (LLM Agent, Claude, GPT-4)
- 명명 규칙: kebab-case
- 필수 섹션: 정의, 관련 연구, 참조

### Concepts (개념)
- 연구 개념 (Emotion Vector, Activation Steering)
- 명명 규칙: kebab-case
- 필수 섹션: 정의, 방법론, 응용

### Sources (소스)
- 원본 문서 (논문, 기사)
- 명명 규칙: YYYY-MM-DD-제목
- 필수 섹션: 요약, 인사이트, 응용

### Queries (질의 결과)
- 사용자 질의에서 생성된 유용한 분석
- 명명 규칙: 주제-설명
- 필수 섹션: 질문, 답변, 참조

## 워크플로우

### Ingest
1. 논문 수집 → sources/에 페이지 생성
2. 관련 entities/ 업데이트
3. 관련 concepts/ 업데이트
4. index.md 업데이트
5. log.md에 항목 추가

### Query
1. index.md에서 관련 페이지 검색
2. 페이지 읽기 및 종합
3. 답변 생성 + 인용
4. 유용하면 queries/에 저장

### Lint
- 주 1회 실행
- 모순, 고아 페이지, 누락 참조 체크
```

### Phase 2: 자동화 스크립트 (2주)

**2.1 Wiki 업데이트 자동화**

`update_wiki.py`:
```python
#!/usr/bin/env python3
"""논문 수집 시 자동으로 wiki 업데이트"""

def ingest_paper_to_wiki(paper):
    # 1. Source 페이지 생성
    create_source_page(paper)
    
    # 2. 엔티티 추출 및 업데이트
    entities = extract_entities(paper)
    for entity in entities:
        update_entity_page(entity, paper)
    
    # 3. 개념 추출 및 업데이트
    concepts = extract_concepts(paper)
    for concept in concepts:
        update_concept_page(concept, paper)
    
    # 4. Index 업데이트
    update_index(paper, entities, concepts)
    
    # 5. Log 추가
    append_to_log("ingest", paper['title'])

def create_source_page(paper):
    """sources/YYYY-MM-DD-제목.md 생성"""
    filename = f"sources/{paper['date']}-{slugify(paper['title'])}.md"
    
    content = f"""# {paper['title']}

**arXiv**: {paper['arxiv_id']}  
**Date**: {paper['date']}  
**Authors**: {', '.join(paper['authors'])}

## Summary
{paper['summary']}

## Insights
{format_insights(paper['insights'])}

## Applications
{format_applications(paper['applications'])}

## Related
- Entities: {format_entities(paper['entities'])}
- Concepts: {format_concepts(paper['concepts'])}
"""
    
    write_file(filename, content)
```

**2.2 검색 기능 구현**

`search_wiki.py`:
```python
#!/usr/bin/env python3
"""Wiki 검색 (간단 버전, 나중에 qmd로 교체)"""

def search_wiki(query):
    # 1. index.md에서 관련 페이지 찾기
    index = read_file('wiki/index.md')
    relevant = extract_relevant_pages(index, query)
    
    # 2. 각 페이지 읽기
    results = []
    for page in relevant:
        content = read_file(f"wiki/{page['path']}")
        results.append({
            'page': page,
            'content': content,
            'relevance': compute_relevance(content, query)
        })
    
    # 3. 관련성 순 정렬
    results.sort(key=lambda x: x['relevance'], reverse=True)
    
    return results
```

### Phase 3: 기존 데이터 마이그레이션 (1주)

**3.1 일일 요약 → Wiki 변환**

```python
def migrate_daily_summaries():
    """기존 daily/ 요약을 wiki로 마이그레이션"""
    daily_dir = '/storage/B8AC-56F1/papers/daily/'
    
    for file in os.listdir(daily_dir):
        if file.endswith('.md') and not file.startswith('TEST'):
            # 1. 파일 읽기
            content = read_file(os.path.join(daily_dir, file))
            
            # 2. 파싱
            paper = parse_daily_summary(content)
            
            # 3. Wiki로 변환
            ingest_paper_to_wiki(paper)
    
    print(f"마이그레이션 완료: {len(files)}개")
```

### Phase 4: qmd 통합 (1주)

**4.1 qmd 설치 및 설정**

```bash
# qmd 설치
pip install qmd

# 인덱스 생성
qmd index wiki/ --output .qmd-index

# MCP server 설정 (OpenClaw용)
qmd serve --port 8080
```

**4.2 검색 API 통합**

```python
def search_wiki_with_qmd(query):
    """qmd MCP server로 검색"""
    # MCP tool 사용
    results = mcp_call('qmd', 'search', {
        'query': query,
        'path': 'wiki/',
        'limit': 10
    })
    
    return results
```

---

## 📊 기대 효과

### 1. 지식 축적 가속화

**Before (현재)**:
- 논문 수집 → 요약 → 끝
- 다음에 같은 주제 질문 → 다시 처음부터 검색

**After (Wiki)**:
- 논문 수집 → 요약 → Wiki 통합 → 엔티티/개념 업데이트
- 다음에 같은 주제 질문 → Wiki에서 즉시 검색 → 새로운 발견은 다시 Wiki에 저장

### 2. 교차 참조 자동화

**Before**:
- "LLM Agent 관련 논문 뭐 있어?" → 전체 검색 필요

**After**:
- `entities/llm-agent.md`에 이미 정리됨
- 관련 논문, 개념, 응용이 모두 연결됨

### 3. 모순 자동 감지

**Before**:
- "A 논문은 X라고 하는데, B 논문은 Y라고 함" → 수동으로 발견

**After**:
- Lint 실행 시 자동으로 모순 플래깅

### 4. 질의 결과 축적

**Before**:
- "감정 벡터와 행동의 관계 분석해줘" → 일회성 답변

**After**:
- 분석 결과 → `queries/emotion-behavior-comparison.md`에 저장
- 다음에 같은 질문 → Wiki에서 즉시 조회

---

## 🎯 우선순위

### 즉시 도입 (1주 이내)
1. ✅ Wiki 디렉토리 구조 생성
2. ✅ WIKI_SCHEMA.md 작성
3. ✅ index.md, log.md 생성
4. ✅ 기존 daily 요약 마이그레이션

### 단기 도입 (1개월 이내)
5. ⏳ Ingest 자동화 스크립트
6. ⏳ Query 자동화 스크립트
7. ⏳ Lint 자동화 스크립트

### 중기 도입 (3개월 이내)
8. ⏳ qmd 검색 엔진 통합
9. ⏳ Marp 슬라이드 통합
10. ⏳ Dataview 쿼리 기능

---

## 📝 다음 단계

1. **Wiki 구조 설계 회의** - 회장님과 구체화
2. **Schema 초안 작성** - AGENTS.md와 통합 여부 결정
3. **마이그레이션 테스트** - 소수 논문으로 파일럿
4. **자동화 스크립트 개발** - Ingest → Query → Lint
5. **배포 및 문서화** - 사용 가이드 작성

---

**마지막 업데이트**: 2026-04-05  
**작성자**: 티씨오 🤖
