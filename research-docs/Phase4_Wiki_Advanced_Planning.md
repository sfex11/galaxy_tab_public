# Phase 4: Wiki 고도화 + GitHub 연동

**시작일**: 2026-04-05  
**예상 기간**: 1주

---

## 🎯 목표

1. **고아 페이지 연결** - Cross-reference 자동 생성
2. **누락 Entity/Concept 생성** - 자동 페이지 생성
3. **빈 섹션 작성** - LLM으로 내용 생성
4. **qmd 통합** - 검색 엔진 구축
5. **GitHub 연동** - 버전 관리 + 협업 + 백업

---

## 📋 작업 계획

### Task 1: Cross-reference 자동 생성

**목표**: 고아 페이지 65개 연결

**방법**:
1. 각 Source 페이지에서 다른 Source로 링크 추가
2. 같은 Entity/Concept을 공유하는 페이지 연결
3. 유사 키워드 기반 연결

**스크립트**: `cross_reference_wiki.py`

---

### Task 2: 누락 Entity/Concept 페이지 생성

**목표**: 12개 누락 참조 해결

**방법**:
1. Lint에서 발견된 누락 페이지 목록 추출
2. 자동으로 Entity/Concept 페이지 생성
3. 기본 템플릿 적용

**스크립트**: `create_missing_pages.py`

---

### Task 3: 빈 섹션 작성

**목표**: 78개 빈 섹션 작성

**방법**:
1. "_필요_", "_없음_" 섹션 찾기
2. Claude로 내용 생성
3. Wiki 페이지 업데이트

**스크립트**: `fill_empty_sections.py`

---

### Task 4: qmd 검색 엔진

**목표**: Wiki 검색 고도화

**방법**:
1. qmd 설치
2. Wiki 인덱스 생성
3. 검색 API 통합

---

### Task 5: GitHub 연동

**목표**: Wiki를 Git으로 관리

**방법**:
1. Git 초기화
2. GitHub 리포지토리 생성
3. 자동 커밋/푸시 스크립트
4. GitHub Pages 호스팅 (선택)

---

## 🛠️ GitHub 활용 전략

### 1. 리포지토리 구조

```
openclaw-wiki/
├── wiki/
│   ├── WIKI_SCHEMA.md
│   ├── index.md
│   ├── log.md
│   ├── entities/
│   ├── concepts/
│   ├── sources/
│   └── queries/
├── scripts/
│   ├── ingest_wiki.py
│   ├── query_wiki.py
│   ├── lint_wiki.py
│   ├── migrate_to_wiki.py
│   ├── cross_reference_wiki.py
│   ├── create_missing_pages.py
│   ├── fill_empty_sections.py
│   └── git_sync.sh
├── .github/
│   └── workflows/
│       └── wiki-sync.yml  # 자동 동기화
├── README.md
└── .gitignore
```

### 2. Git 워크플로우

**자동 커밋**:
- 매일 Wiki 업데이트 시 자동 커밋
- 커밋 메시지: `[auto] Wiki update - YYYY-MM-DD`

**자동 푸시**:
- 커밋 후 GitHub로 푸시
- 충돌 시 알림

**브랜치 전략**:
- `main`: 운영 Wiki
- `dev`: 실험적 변경
- PR로 병합

### 3. GitHub Actions 자동화

**워크플로우**:
```yaml
name: Wiki Sync

on:
  schedule:
    - cron: '0 19 * * *'  # 매일 19:00 UTC
  workflow_dispatch:  # 수동 실행

jobs:
  sync:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      
      - name: Setup Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.11'
      
      - name: Install dependencies
        run: |
          pip install -r requirements.txt
      
      - name: Run Wiki Ingest
        run: |
          python scripts/ingest_wiki.py --latest
      
      - name: Run Wiki Lint
        run: |
          python scripts/lint_wiki.py
      
      - name: Commit changes
        run: |
          git config --local user.email "action@github.com"
          git config --local user.name "GitHub Action"
          git add -A
          git commit -m "[auto] Wiki update - $(date +%Y-%m-%d)" || echo "No changes"
          git push
```

### 4. GitHub Pages 호스팅

**설정**:
1. Settings → Pages
2. Source: main branch
3. Theme: Minimal

**URL**: `https://username.github.io/openclaw-wiki/`

**장점**:
- Wiki를 웹에서 볼 수 있음
- Obsidian Web과 연동 가능
- 공유 가능

### 5. 협업 기능

**Pull Request**:
- 새 소스 추가 → PR 생성
- 리뷰 후 병합

**Issues**:
- Wiki 개선 제안
- 버그 리포트

**Wiki Discussions**:
- 논의 스레드
- Q&A

### 6. 백업 및 복구

**자동 백업**:
- 매일 GitHub에 푸시 = 자동 백업
- 히스토리 관리

**복구**:
```bash
git checkout <commit-hash>
```

### 7. 통계 및 분석

**Git 로그 분석**:
```bash
# Wiki 성장 추이
git log --oneline --since="2026-03-01" | wc -l

# 파일별 변경 횟수
git log --name-only --pretty=format: | sort | uniq -c | sort -rg | head -10

# 기여자 통계
git shortlog -sn
```

---

## 🔧 스크립트 구현 계획

### 1. cross_reference_wiki.py

**기능**:
- 유사 키워드 기반 링크 추가
- 같은 Entity/Concept 공유 페이지 연결

**알고리즘**:
```python
def find_similar_pages(page, all_pages):
    """유사한 페이지 찾기"""
    similar = []
    page_entities = extract_entities(page)
    page_concepts = extract_concepts(page)
    
    for other in all_pages:
        if other == page:
            continue
        
        other_entities = extract_entities(other)
        other_concepts = extract_concepts(other)
        
        # Entity/Concept 교집합
        common_entities = set(page_entities) & set(other_entities)
        common_concepts = set(page_concepts) & set(other_concepts)
        
        if common_entities or common_concepts:
            similar.append({
                'page': other,
                'common_entities': common_entities,
                'common_concepts': common_concepts
            })
    
    return similar

def add_cross_references(page_path, similar_pages):
    """페이지에 cross-reference 추가"""
    with open(page_path, 'a') as f:
        f.write("\n## 관련 문서\n")
        for sim in similar_pages:
            f.write(f"- [[{sim['page']}]]\n")
```

### 2. create_missing_pages.py

**기능**:
- Lint 결과에서 누락 페이지 추출
- 자동 생성

**알고리즘**:
```python
def create_missing_entity(entity_name):
    """누락된 Entity 페이지 생성"""
    template = f"""# {entity_name}

**카테고리**: 미분류  
**생성일**: {datetime.now().strftime('%Y-%m-%d')}

## 정의

_정의 필요_

## 핵심 특성

- 특성 1
- 특성 2

## 관련 연구

_자동 수집 중_

## 메모

_자동 생성됨_
"""
    
    filepath = ENTITIES_DIR / f"{slugify(entity_name)}.md"
    write_file(filepath, template)

def create_missing_concept(concept_name):
    """누락된 Concept 페이지 생성"""
    # 유사하게 구현
    pass
```

### 3. fill_empty_sections.py

**기능**:
- 빈 섹션 찾기
- Claude로 내용 생성

**알고리즘**:
```python
def find_empty_sections(page_path):
    """빈 섹션 찾기"""
    with open(page_path) as f:
        content = f.read()
    
    empty = []
    for match in re.finditer(r'## (.+)\n(_필요_|_없음_|_자동 생성됨_)', content):
        empty.append({
            'section': match.group(1),
            'start': match.start(),
            'end': match.end()
        })
    
    return empty

def fill_section_with_llm(page_path, section_name, context):
    """Claude로 섹션 작성"""
    prompt = f"""
    다음 Wiki 페이지의 "{section_name}" 섹션을 작성하세요.
    
    페이지 제목: {page_path.stem}
    컨텍스트: {context}
    
    2-3문장으로 간결하게 작성하세요.
    """
    
    result = subprocess.run(
        ['claude', '--permission-mode', 'bypassPermissions', '--print', prompt],
        capture_output=True,
        text=True
    )
    
    return result.stdout
```

### 4. git_sync.sh

**기능**:
- Wiki 변경사항 자동 커밋/푸시

```bash
#!/bin/bash

WIKI_DIR="$HOME/.openclaw/workspace/wiki"
LOG_FILE="/storage/B8AC-56F1/papers/cron-git-sync.log"

echo "[$(date)] Git sync 시작" >> "$LOG_FILE"

cd "$WIKI_DIR"

# 변경사항 확인
if git diff --quiet && git diff --staged --quiet; then
    echo "[$(date)] 변경사항 없음" >> "$LOG_FILE"
    exit 0
fi

# 커밋
git add -A
git commit -m "[auto] Wiki update - $(date +%Y-%m-%d)" >> "$LOG_FILE" 2>&1

# 푸시
git push origin main >> "$LOG_FILE" 2>&1

echo "[$(date)] Git sync 완료" >> "$LOG_FILE"
```

---

## 📅 실행 계획

### Week 1: Phase 4 완료

| 일차 | 작업 | 산출물 |
|------|------|--------|
| 1일 | Cross-reference 스크립트 | cross_reference_wiki.py |
| 2일 | 누락 페이지 생성 스크립트 | create_missing_pages.py |
| 3일 | 빈 섹션 작성 스크립트 | fill_empty_sections.py |
| 4일 | Git 초기화 + GitHub 연동 | git_sync.sh |
| 5일 | GitHub Actions 설정 | wiki-sync.yml |
| 6일 | qmd 설치 및 통합 | qmd 설정 |
| 7일 | 통합 테스트 + cron 등록 | cron-git-sync |

---

## 🎯 완료 기준

1. ✅ 고아 페이지 < 10개
2. ✅ 누락 참조 0개
3. ✅ 빈 섹션 < 10개
4. ✅ GitHub 자동 동기화 작동
5. ✅ qmd 검색 기능 작동

---

## 📚 참조

- [Karpathy LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- [qmd](https://github.com/tobi/qmd)
- [GitHub Actions](https://docs.github.com/en/actions)
- [Obsidian Git](https://github.com/denolehov/obsidian-git)

---

**마지막 업데이트**: 2026-04-05  
**작성자**: 티씨오 🤖
