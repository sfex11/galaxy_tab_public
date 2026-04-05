# Wiki Log

**시작일**: 2026-04-05  
**상태**: 활성

---

## [2026-04-05 09:50] init | Wiki 시스템 초기화 완료
- Wiki 디렉토리 구조 생성 완료
  - entities/, concepts/, sources/, queries/
- WIKI_SCHEMA.md 작성 (v1.0, 10.5KB)
- index.md 생성
- log.md 생성 (이 파일)
- Phase 1: Wiki 구조 설계 시작

## [2026-04-05 09:56] ingest | 첫 번째 엔티티 & 컨셉 생성
- Entity 생성: entities/llm-agent.md (1.2KB)
  - LLM 기반 자율 에이전트 정의
  - 관련 연구 주제 정리
- Concept 생성: concepts/emotion-vector.md (1.6KB)
  - 감정 벡터 정의 및 작동 원리
  - 한국 특화 감정 개념 추가
  - Anthropic 2026 연구 요약
- Index 업데이트: entities (+1), concepts (+1)
- 총 2개 페이지 생성

---

## 사용법

**파싱 예시**:
```bash
# 최근 5개 항목
grep "^## \[" log.md | tail -5

# 오늘 작업
grep "^\[2026-04-05" log.md

# Ingest만 보기
grep "ingest |" log.md

# Query만 보기
grep "query |" log.md

# Lint만 보기
grep "lint |" log.md
```

---

_이 파일은 append-only로 운영됩니다._

## [2026-04-05 09:58] ingest | ActionParty: Multi-Subject Action Binding in Generative Video Games

## [2026-04-05 10:02] lint | Wiki 건전성 체크
- Issues: 15개
- Orphans: 3, Missing: 12, Contradictions: 0

## [2026-04-05 11:09] migrate | 61개 파일 마이그레이션 완료 (2개 스킵)

## [2026-04-05 11:10] migrate | 1개 파일 마이그레이션 완료 (62개 스킵)

## [2026-04-05 11:11] lint | Wiki 건전성 체크
- Issues: 77개
- Orphans: 65, Missing: 12, Contradictions: 0

## [2026-04-05 11:50] cross-ref | 45개 페이지 연결

## [2026-04-05 14:04] cross-ref | 0개 페이지 연결

## [2026-04-05 16:00] cross-ref | 0개 페이지 연결
