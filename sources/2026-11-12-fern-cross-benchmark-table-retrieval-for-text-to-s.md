# FERN: Cross-Benchmark Table Retrieval for Text-to-SQL with Frozen Retrievers and Learned Ranking

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14477v1

## 💡 핵심 인사이트

테이블 검색의 품질 병목이 검색기 자체가 아니라 후보 정렬 계층에 있으며, 이 정렬은 생성적 LLM 없이 구조적 피처와 경량 학습 랭커로 대체 가능하다.

## 📖 분석

# FERN: Cross-Benchmark Table Retrieval for Text-to-SQL

대규모 풀드 카탈로그(BIRD·Spider·Fiben)에서 질의에 필요한 테이블을 선검색해야 한다는 text-to-SQL의 상류 병목을 다룬다. RASL이 Claude 3.5로 키워드 추출·테이블 선택을 수행하는 것과 대비해, FERN은 3개의 동결(frozen) 검색기를 융합해 100개 후보를 생성하고, 후보별 최대 120개 피처를 기술한 뒤 BIRD 훈련 질의로 한 번 학습한 LightGBM 랭커로 재정렬한다.

## 기존 Wiki와의 관계

- [[text-to-sql]]: TeCoD가 반복 질의의 SQL 생성 병목을 제약 디코딩으로 풀었다면, FERN은 그 이전 계층인 카탈로그 테이블 검색 병목을 규정한다. 생성 전 파이프라인의 검색·생성 양 계층이 모두 비생성적 해법으로 대체되는 흐름을 형성한다.
- [[slm-reasoning-gap]]: 생성적 LLM을 피처 엔지니어링 + 경량 학습 랭커로 대체하는 '추론 필요성 제거' 경로의 검색 도메인 실증이다.
- [[retrieval-augmented-generation]]: 단일 검색기가 아닌 다중 동결 검색기 융합 + 학습된 정렬 계층의 2단 구조를 제시한다. 검색기는 동결하고 정렬만 학습하는 분할은 [[router-within]]·RICE 계열의 '동결 모델 유도'와 대비되는 '동결+학습 하이브리드' 축을 추가한다.
- [[transfer-learning]]: BIRD 질의로 학습한 랭커가 교차 벤치마크 풀드 카탈로그로 전이되는 사례를 제공한다.

## 🔗 관련 논문

- Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy
- Distill Globally, Adapt Locally: Reasoning Distillation and Product-Type Specialization
- Effective Dense Retrieval using Only In-Context Examples
- The Router Within: Eliciting Native Skill Routing from a Frozen LLM
- Superintelligent Retrieval Agent: The Next Frontier of Information Retrieval

## 🏷️ 엔티티

- [[entities/fern.md|fern]]
- [[entities/text-to-sql.md|text-to-sql]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/transfer-learning.md|transfer-learning]]

## 📐 개념

- [[concepts/table-retrieval.md|table-retrieval]]
- [[concepts/frozen-retriever-fusion.md|frozen-retriever-fusion]]
- [[concepts/feature-engineered-ranking.md|feature-engineered-ranking]]
- [[concepts/cross-benchmark-ranking-transfer.md|cross-benchmark-ranking-transfer]]

---
_LLM 분석으로 생성됨_
