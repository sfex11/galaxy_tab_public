# sparse-attention-unification

**카테고리**: 미분류
**생성일**: 2026-05-01

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-01-unifying-sparse-attention-with-hierarchical-memory.md|Unifying Sparse Attention with Hierarchical Memory for Scala]]

### On-Demand Attention: Language Models Know When to Recall (2026-09-19)

희소 어텐션의 선택 기준을 정적 패턴(지역성·계층 메모리)에서 동적 필요성 예측으로 이동시킨다. 무엇을 건너뛸지가 아니라 언제 읽을지를 예측하는 대안 축을 희소성 스펙트럼에 추가한다.

### On-Demand Attention: Language Models Know When to Recall (2026-09-21)

기존 노트의 '동적 필요성 예측' 축을 [[concepts/local-sufficiency.md|local sufficiency]] 및 [[concepts/expected-value-of-information.md|expected value of information]]과 연결해 심화한다 — 필요성 판정이 학습된 EVI 추정기(recall head)로 구현될 때, 희소성은 건너뛰기 전략이 아니라 읽기의 기대 이익 관리 문제로 재정의된다.

### Latent Sparse Attention: Towards Subquadratic Ultra-Long Context Atten (2026-11-03)

Latent Sparse Attention은 계층적 메모리 기반 희소 어텐션과 병렬되는 '잠재 투영 기반' 축을 추가한다. 인덱싱의 검색 공간을 토큰 수준 KV 캐시에서 학습된 잠재 상태로 이동시켜, 정적 구조(계층) vs 학습된 표현(잠재 투영)이라는 희소성 확보의 두 경로가 병치됨을 보여준다.

→ [[sources/2026-11-03-latent-sparse-attention-towards-subquadratic-ultra.md|상세 보기]]

### Subquadratic Attention with a Hierarchical Tree-Structured Indexer (2026-11-03)

본 논문은 통합 희소 어텐션 계열의 구조적 한계 — 인덱서 자체의 2차 스케일링 — 를 트리 구조로 돌파하여, 희소성 접근이 '상수배 가속'에서 '점근적 병목 제거'로 격상될 수 있음을 보여준다. 계층 구조의 역할이 메모리 저장 조직에서 조회 탐색 구조로 분화함을 제시한다.

→ [[sources/2026-11-03-subquadratic-attention-with-a-hierarchical-tree-st.md|상세 보기]]

### CISA: Retrofitting Dense Attention Models with Chunk-Indexed Sparse At (2026-11-04)

희소 어텐션 통합 논의에 '학습 없는 개조(retrofit)' 경로를 제공한다. 학습된 계층적 메모리를 전제하던 기존 방향과 달리, 사전학습 dense 모델을 그래디언트 없이 희소화함으로써 희소화의 적용 시점이 학습에서 추론으로 확장됨을 시사한다.

→ [[sources/2026-11-04-cisa-retrofitting-dense-attention-models-with-chun.md|상세 보기]]
