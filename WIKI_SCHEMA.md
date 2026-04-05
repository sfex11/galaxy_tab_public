# Wiki Schema

**버전**: 1.0  
**생성일**: 2026-04-05  
**목적**: OpenClaw LLM Wiki 운영 규칙 정의

---

## 📁 디렉토리 구조

```
wiki/
├── index.md              # 전체 콘텐츠 카탈로그
├── log.md                # 작업 타임라인
├── entities/             # 엔티티 페이지
│   ├── llm-agent.md
│   ├── emotion-vector.md
│   └── ...
├── concepts/             # 개념 페이지
│   ├── activation-steering.md
│   ├── representation-engineering.md
│   └── ...
├── sources/              # 원본 소스 요약
│   ├── 2026-04-03-ActionParty.md
│   ├── 2026-04-04-Steerable.md
│   └── ...
├── queries/              # 질의 결과
│   ├── emotion-behavior-comparison.md
│   └── ...
└── WIKI_SCHEMA.md        # 이 파일
```

---

## 📄 페이지 타입

### 1. Entities (엔티티)

**정의**: 연구 대상이 되는 구체적 객체

**예시**:
- `llm-agent.md` - LLM 기반 자율 에이전트
- `emotion-vector.md` - 감정 개념의 선형 표현
- `claude-3.5.md` - Claude 3.5 모델
- `openclaw.md` - OpenClaw 시스템

**필수 섹션**:
```markdown
# Entity Name

## 정의
[간단한 정의, 1-2문장]

## 핵심 특성
- 특성 1
- 특성 2
- 특성 3

## 관련 연구
- [[sources/2026-04-03-ActionParty]] - 다중 에이전트 제어
- [[sources/2026-04-04-Steerable]] - 조향 가능한 표현

## 관련 개념
- [[concepts/activation-steering]]
- [[concepts/representation-engineering]]

## 참조
- 외부 링크
- 관련 문서
```

**명명 규칙**: 
- kebab-case (소문자 + 하이픈)
- 예: `llm-agent`, `emotion-vector`

---

### 2. Concepts (개념)

**정의**: 연구에서 사용되는 추상적 개념이나 방법론

**예시**:
- `activation-steering.md` - 활성화 조향
- `representation-engineering.md` - 표현 엔지니어링
- `emotion-vector.md` - 감정 벡터
- `causal-tracing.md` - 인과 추적

**필수 섹션**:
```markdown
# Concept Name

## 정의
[개념의 정의]

## 방법론
[어떻게 작동하는지]

## 응용 분야
- 응용 1
- 응용 2

## 관련 엔티티
- [[entities/llm-agent]]
- [[entities/claude-3.5]]

## 관련 소스
- [[sources/2026-04-03-Paper1]]
- [[sources/2026-04-04-Paper2]]

## 참조
- 논문 링크
- 블로그 포스트
```

**명명 규칙**:
- kebab-case
- 예: `activation-steering`, `representation-engineering`

---

### 3. Sources (소스)

**정의**: 원본 문서의 요약 (논문, 기사, 책 등)

**예시**:
- `2026-04-03-ActionParty.md` - ActionParty 논문
- `2026-04-04-Steerable.md` - Steerable 논문
- `2026-04-05-Wiki-Pattern.md` - Karpathy Wiki 패턴

**필수 섹션**:
```markdown
# Source Title

**타입**: 논문 | 기사 | 책 | 문서  
**출처**: arXiv, 웹, 책  
**날짜**: YYYY-MM-DD  
**링크**: URL (있는 경우)

## 핵심 요약
[300자 이내 요약]

## 주요 내용
### 섹션 1
[내용]

### 섹션 2
[내용]

## 인사이트
1. [인사이트 1]
2. [인사이트 2]
3. [인사이트 3]

## 응용 가능성
1. [응용 1]
2. [응용 2]

## 추출된 엔티티
- [[entities/entity1]]
- [[entities/entity2]]

## 추출된 개념
- [[concepts/concept1]]
- [[concepts/concept2]]

## 관련 소스
- [[sources/related-source1]]
- [[sources/related-source2]]
```

**명명 규칙**:
- `YYYY-MM-DD-제목-간소화.md`
- 예: `2026-04-03-ActionParty.md`

---

### 4. Queries (질의 결과)

**정의**: 사용자 질의에서 생성된 유용한 분석 결과

**예시**:
- `emotion-behavior-comparison.md` - 감정-행동 비교 분석
- `trend-analysis-2026-q1.md` - 2026 Q1 트렌드 분석

**필수 섹션**:
```markdown
# Query Result Title

**질문**: [원래 사용자 질문]  
**날짜**: YYYY-MM-DD  
**관련도**: 높음 | 보통 | 낮음

## 답변
[종합 답변]

## 분석 과정
1. [단계 1]
2. [단계 2]
3. [단계 3]

## 핵심 발견
- 발견 1
- 발견 2
- 발견 3

## 참조 페이지
- [[entities/entity1]]
- [[concepts/concept1]]
- [[sources/source1]]

## 후속 질문
- [탐색할 만한 추가 질문]
```

**명명 규칙**:
- 주제-설명.md
- 예: `emotion-behavior-comparison.md`

---

## 🔄 워크플로우

### Workflow 1: Ingest (섭취)

**트리거**: 새 논문/기사 수집

**프로세스**:
1. **소스 페이지 생성**
   - `sources/YYYY-MM-DD-제목.md` 작성
   - 요약, 인사이트, 응용 작성

2. **엔티티 추출 및 업데이트**
   ```python
   entities = extract_entities(source)
   for entity in entities:
       if not exists(f"entities/{entity}.md"):
           create_entity_page(entity)
       update_entity_page(entity, source)
   ```

3. **개념 추출 및 업데이트**
   ```python
   concepts = extract_concepts(source)
   for concept in concepts:
       if not exists(f"concepts/{concept}.md"):
           create_concept_page(concept)
       update_concept_page(concept, source)
   ```

4. **Index 업데이트**
   - 해당 카테고리에 새 항목 추가
   - 링크 + 1줄 요약

5. **Log 추가**
   ```markdown
   ## [YYYY-MM-DD HH:MM] ingest | Source Title
   - Source 페이지 생성: sources/YYYY-MM-DD-Title.md
   - Entity 업데이트: entity1, entity2
   - Concept 업데이트: concept1, concept2
   ```

**하나의 소스 → 10-15개 페이지 터치**

---

### Workflow 2: Query (질의)

**트리거**: 사용자 질문

**프로세스**:
1. **Index에서 관련 페이지 검색**
   ```python
   def search_index(query):
       index = read_file('index.md')
       relevant = []
       for line in index:
           if matches_query(line, query):
               relevant.append(extract_page_link(line))
       return relevant
   ```

2. **페이지 읽기**
   ```python
   pages = []
   for page_link in relevant_pages:
       content = read_file(page_link)
       pages.append(content)
   ```

3. **답변 종합**
   ```python
   answer = synthesize(query, pages)
   ```

4. **인용 추가**
   ```markdown
   답변 텍스트...

   **출처**:
   - [[entities/entity1]]
   - [[sources/source1]]
   ```

5. **유용한 답변 → Wiki에 저장**
   ```python
   if is_valuable(answer):
       create_query_result(answer)
       update_index(answer)
       append_log("query", question)
   ```

---

### Workflow 3: Lint (건전성 체크)

**트리거**: 주 1회 자동 또는 수동

**체크 항목**:

1. **모순 검사**
   ```python
   contradictions = []
   for entity in all_entities:
       claims = extract_claims(entity)
       for i, claim1 in enumerate(claims):
           for claim2 in claims[i+1:]:
               if is_contradiction(claim1, claim2):
                   contradictions.append((entity, claim1, claim2))
   ```

2. **고아 페이지 (Orphan Pages)**
   ```python
   orphans = []
   for page in all_pages:
       inbound_links = count_inbound_links(page)
       if inbound_links == 0:
           orphans.append(page)
   ```

3. **누락된 참조**
   ```python
   missing_refs = []
   for page in all_pages:
       for link in extract_links(page):
           if not page_exists(link):
               missing_refs.append((page, link))
   ```

4. **오래된 정보**
   ```python
   stale = []
   for page in all_pages:
       last_updated = get_last_updated(page)
       if days_since(last_updated) > 90:
           stale.append(page)
   ```

5. **개선 제안**
   ```python
   suggestions = []
   # 중요 개념인데 페이지가 없는 경우
   # 크로스레퍼런스가 부족한 경우
   # 요약이 너무 짧은 경우
   ```

**결과 보고**:
```markdown
# Lint Report - YYYY-MM-DD

## Issues Found
- ❌ 3 contradictions
- ⚠️  5 orphan pages
- ⚠️  2 missing references
- ℹ️  10 stale pages

## Suggestions
- Create page for: [[concepts/new-concept]]
- Add cross-reference: [[entities/entity1]] → [[entities/entity2]]
- Update: [[sources/old-source]] (90+ days)

## Actions Taken
- Fixed 2 missing references
- Created 1 missing page
```

---

## 🛠️ 특수 파일

### index.md

**용도**: Wiki 전체 카탈로그

**구조**:
```markdown
# Wiki Index

**마지막 업데이트**: YYYY-MM-DD  
**총 페이지 수**: XX개

---

## Entities (XX)

### LLM & Agents
- [[entities/llm-agent]] - LLM 기반 자율 에이전트
- [[entities/emotion-vector]] - 감정 개념의 선형 표현
- [[entities/claude-3.5]] - Anthropic Claude 3.5

### Systems
- [[entities/openclaw]] - OpenClaw 에이전트 프레임워크
- [[entities/transformer-lens]] - Transformer 해석 도구

---

## Concepts (XX)

### Representation
- [[concepts/activation-steering]] - 활성화 조향 기법
- [[concepts/representation-engineering]] - 표현 엔지니어링
- [[concepts/sparse-autoencoder]] - 희소 오토인코더

### Analysis
- [[concepts/causal-tracing]] - 인과 추적
- [[concepts/probing-classifier]] - 프로빙 분류기

---

## Sources (XX)

### 2026-04
- [[sources/2026-04-03-ActionParty]] - 다중 에이전트 제어
- [[sources/2026-04-04-Steerable]] - 조향 가능한 표현
- [[sources/2026-04-05-Wiki-Pattern]] - LLM Wiki 패턴

### 2026-03
- [[sources/2026-03-31-Emotion]] - 감정 벡터 연구
- ...

---

## Query Results (XX)

- [[queries/emotion-behavior-comparison]] - 감정-행동 비교 분석
- [[queries/trend-2026-q1]] - 2026 Q1 트렌드
```

**업데이트 규칙**:
- 모든 Ingest 시 해당 섹션에 항목 추가
- 페이지 삭제 시 항목 제거
- 마지막 업데이트 날짜 갱신

---

### log.md

**용도**: Wiki 진화 타임라인

**구조**:
```markdown
# Wiki Log

**시작일**: 2026-04-05

---

## [2026-04-05 09:45] ingest | ActionParty: Multi-Subject Action Binding
- Source 페이지 생성: sources/2026-04-03-ActionParty.md
- Entity 생성: entities/llm-agent.md
- Concept 생성: concepts/multi-agent-control.md
- Index 업데이트: entities (+1), concepts (+1), sources (+1)

## [2026-04-05 10:15] query | "감정 벡터가 행동에 미치는 영향은?"
- 검색: entities/emotion-vector.md, concepts/activation-steering.md
- 답변 생성 완료
- Query 결과 저장: queries/emotion-behavior-comparison.md

## [2026-04-05 11:00] lint | 전체 Wiki 건전성 체크
- Issues: 0 contradictions, 2 orphans, 1 missing ref
- Actions: Fixed 1 missing ref
- Suggestions: Create page for concepts/new-concept
```

**파싱 가능**:
```bash
# 최근 5개 항목
grep "^## \[" log.md | tail -5

# 오늘 작업
grep "^\[2026-04-05" log.md

# Ingest만 보기
grep "ingest |" log.md
```

---

## 🎨 템플릿

### Entity 템플릿

```markdown
# Entity Name

**카테고리**: LLM | System | Tool | Concept  
**생성일**: YYYY-MM-DD  
**최종 수정**: YYYY-MM-DD

## 정의

[1-2문장 정의]

## 핵심 특성

- **특성 1**: 설명
- **특성 2**: 설명
- **특성 3**: 설명

## 관련 연구

- [[sources/YYYY-MM-DD-Paper]] - 간단 설명
- [[sources/YYYY-MM-DD-Paper2]] - 간단 설명

## 관련 개념

- [[concepts/concept1]] - 관계 설명
- [[concepts/concept2]] - 관계 설명

## 응용 분야

1. **응용 1**: 설명
2. **응용 2**: 설명

## 외부 참조

- [링크 텍스트](URL)
- [링크 텍스트 2](URL2)

## 메모

[추가 노트]
```

### Concept 템플릿

```markdown
# Concept Name

**분야**: Representation | Analysis | Control  
**생성일**: YYYY-MM-DD  
**최종 수정**: YYYY-MM-DD

## 정의

[개념 정의]

## 작동 원리

### 단계 1
[설명]

### 단계 2
[설명]

### 단계 3
[설명]

## 방법론

```python
# 코드 예시 (해당하는 경우)
def example():
    pass
```

## 장점

- 장점 1
- 장점 2
- 장점 3

## 한계

- 한계 1
- 한계 2

## 관련 엔티티

- [[entities/entity1]] - 관계 설명
- [[entities/entity2]] - 관계 설명

## 관련 소스

- [[sources/YYYY-MM-DD-Paper]] - 핵심 기여
- [[sources/YYYY-MM-DD-Paper2]] - 확장 연구

## 참조

- [논문 링크](URL)
- [블로그 포스트](URL)
```

---

## 📏 규칙

### 링크 규칙

**내부 링크**:
- `[[entities/page-name]]` - 다른 wiki 페이지
- `[[sources/2026-04-03-Paper]]` - 소스 페이지

**외부 링크**:
- `[링크 텍스트](https://url.com)`

### 태그 규칙

**YAML Frontmatter** (선택사항):
```markdown
---
tags: [emotion, llm, steering]
created: 2026-04-05
updated: 2026-04-05
importance: high
---
```

### 명명 규칙

**파일명**:
- kebab-case only
- 영어 소문자 + 숫자 + 하이픈
- 예: `llm-agent.md`, `activation-steering.md`

**페이지 제목**:
- 자유 형식
- 명확하고 간결하게

---

## 🔄 유지보수

### 일일 작업
- 새 소스 Ingest
- Query 결과 저장
- Log 업데이트

### 주간 작업
- Lint 실행 (일요일)
- Orphan pages 처리
- Stale pages 업데이트

### 월간 작업
- 전체 구조 검토
- Schema 업데이트
- 중요 페이지 개선

---

## 📊 메트릭

추적할 지표:
- **총 페이지 수**: XX개
- **평균 업데이트 빈도**: XX일
- **교차 참조 수**: XX개
- **Orphan pages**: XX개
- **모순 수**: XX개

---

## 🔧 도구

### 필수
- Markdown 에디터 (Obsidian 권장)
- Git (버전 관리)

### 권장
- qmd (검색 엔진)
- Marp (슬라이드)
- Dataview (쿼리)

---

## 📚 참조

- [Karpathy's LLM Wiki Pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- [Obsidian](https://obsidian.md/)
- [qmd](https://github.com/tobi/qmd)

---

**마지막 업데이트**: 2026-04-05  
**버전**: 1.0
