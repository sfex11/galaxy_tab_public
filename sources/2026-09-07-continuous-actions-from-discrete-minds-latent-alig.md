# Continuous Actions from Discrete Minds: Latent-Aligned Planning for End-to-End Autonomous Driving

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04070v1

## 💡 핵심 인사이트

사고-행동 간극은 능력 문제가 아닌 표현 형식 문제이며, VQ-VAE 잠재 공간이라는 공유 인터페이스를 통해 이산적 의미 추론과 연속적 물리 실행이 번역이 아닌 공존으로 해소될 수 있다.

## 📖 분석

LaPla는 VLM의 이산 토큰 추론과 자율주행의 연속적·물리제약 실행 사이 간극을 잠재 정렬로 봉합하는 통합 VLA 프레임워크다. 핵심 메커니즘은 잔여 벡터 양자화 VQ-VAE 기반 액션 토크나이저로, 차량 운동학을 이산 토큰 시퀀스로 인코딩하여 VLM이 자연어 추론과 동일한 형식으로 운동 계획을 생성하게 한다.

Wiki 누적 관점에서 이 논문의 위치는 두 축으로 정리된다. 첫째, 사고-행동 간극([[thinking-acting-gap]])의 물리 도메인 확장이다. VLM의 이산 추론과 차량의 연속 동역학 사이 간극의 근원이 능력 부족이 아닌 표현 형식의 비동형성임을 입증하고, 해법이 모델을 연속화하거나 세계를 이산화하는 것이 아니라 두 체계가 공존하는 잠재 인터페이스 구축임을 제시한다. 이는 [[representation-action-gap]]이 도구 호출에서, [[algorithm-system-translation-gap]]이 시스템 번역에서 각각 진단한 동일 구조의 물리적 발현이다.

둘째, VLA 훈련의 도메인 확장이다. [[vla-foundry]]가 로봇 조작에서 VLA 통합 훈련을 정의했다면, LaPla는 [[end-to-end-vla-training]]이 차량 제어라는 더 연속적인 도메인으로 확장 가능함을 실증하여 VLA 패러다임의 도메인 불변성을 검증한다. [[tokenization]]과 [[vector-quantization]]이 단순 압축 기법이 아니라 '물리 제약의 이산 인코딩'이라는 표현 계약으로 재정의된다는 점이 이 논문의 고유한 기여다.

## 🔗 관련 논문

- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- VLA Foundry: A Unified Framework for Training Vision-Languag
- A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia

## 🏷️ 엔티티

- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/action-tokenization.md|action-tokenization]]
- [[entities/latent-aligned-planning.md|latent-aligned-planning]]
- [[entities/representation-action-gap.md|representation-action-gap]]
- [[entities/thinking-acting-gap.md|thinking-acting-gap]]
- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/autonomous-driving.md|autonomous-driving]]

## 📐 개념

- [[concepts/tokenization.md|tokenization]]
- [[concepts/vector-quantization.md|vector-quantization]]
- [[concepts/discrete-continuous-adaptation-transition.md|discrete-continuous-adaptation-transition]]
- [[concepts/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]

---
_LLM 분석으로 생성됨_
