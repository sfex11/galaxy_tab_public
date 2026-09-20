# Deep Noir: Autonomous Steering Discovery via Architectural Chronometry in Transformer Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20722v1

## 💡 핵심 인사이트

표현 수렴 프로파일은 행동과 인과적으로 결합된 동역학 불변량이므로, 이를 판독하는 것만으로 스티어링의 위치·강도가 자동 유도 가능하며 활성화 개입 설계가 수동 장인정신에서 신호 기반 자동화로 전환된다.

## 📖 분석

Deep Noir은 Logit Lens 수렴 프로파일과 인과적 헤드 수준 귀속을 활용해 활성화 스티어링의 위치·강도를 자동 발견하는 프레임워크다. 1B에서 16.7%p, 7-9B에서 21-42%p의 제어 성능 개선을 달성하여 스티어링 설계의 수동 장인정신을 신호 기반 자동화로 전환한다.

기존 축적 대비 세 가지 심화가 있다. 첫째, [[architectural-chronometry]]가 [[dynamical-invariant-monitoring]]과 결합한다 — '언제·어디서 수렴하는가'라는 프로파일은 행동을 산출하는 계산에 인과적으로 묶인 동역학 불변량이므로, 판독 대상이 정적 활성화 값에서 시간적 수렴 구조로 이동한다. 둘째, [[causal-head-level-attribution]]이 [[causal-load-verification]]의 구현체로 기능한다 — 귀속 신호로 개입 지점을 고르는 것은 시그니처의 하중을 행동 변화로 검증하는 경로다. 셋째, 판독(수렴 시각)→파라미터→조작(스티어링 주입)의 직렬 연결이 [[steering-read-manipulation-duality]]의 실용적 완성이자 [[read-to-manipulate-pipeline]]의 실증이다.

대가와 경계도 명확하다: [[read-write-symmetry]]에 따라 수렴 신호로 조작 가능한 자는 같은 신호로 위조도 가능하므로, 감시 응용에는 [[probe-randomization-defense]] 같은 방어자 우위 설계가 전제된다. 또한 개선 폭이 스케일과 함께 증가하는 [[scale-dependent-steering-gains]]는 대형 모델일수록 스티어링 공격 표면이 넓어짐을 의미한다.

## 🔗 관련 논문

- Look Before You Leap: Factual Decoding with Internal Attribution Signal
- Monitoring and Discovering Reward Hacking with Internal Representation
- It's Not RoPE that Creates Sinks: The Role of Self-Concentration and Value Norms

## 🏷️ 엔티티

- [[entities/activation-steering.md|activation-steering]]
- [[entities/architectural-chronometry.md|architectural-chronometry]]
- [[entities/logit-lens-convergence.md|logit-lens-convergence]]
- [[entities/causal-head-level-attribution.md|causal-head-level-attribution]]
- [[entities/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[entities/dynamical-invariant-monitoring.md|dynamical-invariant-monitoring]]
- [[entities/causal-load-verification.md|causal-load-verification]]
- [[entities/read-to-manipulate-pipeline.md|read-to-manipulate-pipeline]]
- [[entities/scale-dependent-steering-gains.md|scale-dependent-steering-gains]]
- [[entities/activation-steering-parameter-automation.md|activation-steering-parameter-automation]]
- [[entities/read-write-symmetry.md|read-write-symmetry]]

## 📐 개념

- [[concepts/architectural-chronometry.md|architectural-chronometry]]
- [[concepts/logit-lens-convergence.md|logit-lens-convergence]]
- [[concepts/logit-lens-convergence-timing.md|logit-lens-convergence-timing]]
- [[concepts/causal-head-level-attribution.md|causal-head-level-attribution]]
- [[concepts/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[concepts/activation-steering-parameter-automation.md|activation-steering-parameter-automation]]
- [[concepts/scale-dependent-steering-gains.md|scale-dependent-steering-gains]]
- [[concepts/dynamical-invariant-monitoring.md|dynamical-invariant-monitoring]]
- [[concepts/causal-load-verification.md|causal-load-verification]]
- [[concepts/read-write-symmetry.md|read-write-symmetry]]
- [[concepts/read-to-manipulate-pipeline.md|read-to-manipulate-pipeline]]

---
_LLM 분석으로 생성됨_
