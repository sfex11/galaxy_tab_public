# distribution-preserving-acceleration

**카테고리**: 미분류
**생성일**: 2026-09-07

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-07-unlocking-lossless-speedups-in-llms-via-discrete-d.md|Unlocking Lossless Speedups in LLMs via Discrete Diffusion]]

### Discrete Beckmann Transport Models for One-Step Language Modeling and  (2026-09-16)

가속이 분포 보존이나 교사 증류를 전제하지 않을 수 있음을 보여준다. DBTM은 기존 분포를 유지하는 대신 고정점 수렴이라는 새 보장 체계를 채택하여 가속-무손실성의 정의 자체를 확장한다.

### Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruning (2026-09-18)

무손실성을 목표로 하는 가속 계열과 대비되는 제3 범주를 연다 — 분포 변경을 의도적으로 수용하되 그 변경을 '품질 지향적 재선택'에 사용하는 축으로, 가속-무손실-품질의 삼각 구도에서 품질 정점의 실현 사례가 된다.

### Watermarkable Multi-Draft Speculative Sampling via Poisson Processes (2026-09-22)

분포 보존 전제의 경계 조건을 명시한다 — 워터마킹은 본질적으로 분포를 변형하므로 무손실 가속과 직접 충돌하며 기존 연구는 결합 불가능으로 판단했다. 다중 드래프트 Poisson 접근은 이 충돌이 드래프트 선택 수준에서 해소 가능함을 보여, 가속-보장 트레이드오프의 정의를 확장한다.

### RheoSampling: Resolving the One-Hot Dilemma in Stochastic Dynamic-Tree (2026-09-22)

가속 기법의 분포 보존 원칙이 인프라 구조 선택에 의해 위반되는 구체적 사례를 제공한다. 트리 구축이 드래프트 분포를 은밀히 변형하는 '구조 유발 분포 붕괴'라는 새로운 위반 유형을 추가한다.

### TextSeal2: Distortion-Free LLM Watermarking with Copula Mixing and Mem (2026-11-02)

왜곡 없는 워터마킹이 타겟 분포 무변경 원칙을 준수해야 수용률 무변경과 추측 디코딩 호환성이 성립함을 보여준다. 분포 보존이 가속뿐 아니라 provenance 신호 유지의 전제조건임으로 확장된다.

→ [[sources/2026-11-02-textseal2-distortion-free-llm-watermarking-with-co.md|상세 보기]]

### Flide: Accelerating Decision Inference with Exact State Forking (2026-11-03)

가속-무손실성의 적용 범위를 토큰 생성과 샘플러 교체에서 트리 구조 결정 추론으로 확장한다. 정확성(exactness)이 출력 확률 보존과 분기 시 접두사 상태 충실도라는 이중 조건을 포괄함을 규정한다.

→ [[sources/2026-11-03-flide-accelerating-decision-inference-with-exact-s.md|상세 보기]]
