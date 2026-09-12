# LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11739v1

## 💡 핵심 인사이트

생성 길이(효율성)와 정렬 품질은 손실 함수 수준에서 상충하지 않을 수 있다 — 업데이트 부공간이라는 파라미터화 차원이 두 목표를 분리된 설계 축으로 만들어, 선호 정렬의 장황함 편향을 손실 수정 없이 제어할 가능성을 연다.

## 📖 분석

# LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Generation

LOCUS는 포스트트레이닝 업데이트의 파라미터화 자체가 생성 길이의 인과적 제어 변수임을 밝힌다. 표준 선호 정렬은 유틸리티 개선 없이 응답을 장황하게 만드는 구조적 경향을 가지며, 본 논문은 손실 함수를 수정하지 않고 태스크 인지 저랭크 적응 부공간을 선택함으로써 유틸리티 제약 하에서 출력 토큰 비용을 최소화한다.

### 기존 Wiki와의 관계

→ **length-inflation**: OPD에서 관찰된 길이 인플레이션의 포스트트레이닝 일반 원리를 제공 — 선호 정렬 자체가 장황함의 원천이며, 제어 지점이 손실이 아닌 파라미터화에 있음을 시사한다.

→ **token-efficiency**: 토큰 효율화의 계층을 입력 측(스키마 지연 로딩), 추론 측(적응적 추론)에 이어 훈련 시점 파라미터화로 확장한다. '불필요한 컨텍스트의 원천 차단' 논리를 '불필요한 출력 길이의 생성 구조 차단'으로 일반화한다.

→ **parameter-decoupling**: 정렬 손실 불변 하에서 업데이트 부공간이 시퀀스 길이를 조정함을 보여, 품질 목표와 비용 목표가 별도 파라미터 축으로 분해 가능함을 확장한다. 이산 확산의 샘플러 교체와 함께 분리 가능성의 두 실증 사례를 형성한다.

→ **model-pruning**: 레이어 입도('무엇이 어느 레이어에 사는가')를 랭크 입도('무엇이 어느 부공간에 사는가')로 확장한다. 기능적 지역화가 희소화와 적응 부공간 선택 양쪽에 공통으로 작동함을 시사한다.

→ **cost-dominance-dimension-asymmetry**: 토큰 소비 총량이 서빙 비용을 직접 지배하는 구조에 대한 훈련 시점 대응을 제공한다.

## 🔗 관련 논문

- Demystifying OPD: Length Inflation and Stabilization Strategies
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion
- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading
- Don't Drop Dropout: Optimizing Layer Sparsity for Efficient
- Forgetting Only What Matters: Layer-Selective Unlearning toward Robust

## 🏷️ 엔티티

- [[entities/post-training.md|post-training]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/length-inflation.md|length-inflation]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/model-pruning.md|model-pruning]]
- [[entities/cost-dominance-dimension-asymmetry.md|cost-dominance-dimension-asymmetry]]
- [[entities/task-aware-subspace-selection.md|task-aware-subspace-selection]]

## 📐 개념

- [[concepts/length-inflation.md|length-inflation]]
- [[concepts/parameter-decoupling.md|parameter-decoupling]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/low-rank-adaptation-subspace.md|low-rank-adaptation-subspace]]
- [[concepts/inference-time-behavior-control.md|inference-time-behavior-control]]

---
_LLM 분석으로 생성됨_
