# TANDEM: Balancing Centralized and Decentralized Critics to Address the Information Gap in Complex Multi-Agent Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37592v1

## 💡 핵심 인사이트

CTDE의 정보 간극은 부분 관측·노이즈·개방성 하에서 구조적으로 확대되며, 해법은 비평자의 제거(회피)가 아니라 정보 조건의 실행 정합화로 성립할 수 있다.

## 📖 분석

TANDEM은 CTDE의 근본 결함 — 전역 상태를 보는 중앙 비평자로 훈련된 정책이 실행 시점에 갖지 못할 정보에 의존하도록 최적화되는 '정보 간극' — 을 정식화하고, 중앙·분산 비평자의 균형으로 해소한다. 본 항목은 2026-10-29 등록분의 갱신이며, 확장된 초록에서 간극의 확대 조건이 3축으로 명시된다: 부분 관측, 관측 노이즈, 그리고 실행 중 에이전트·태스크 집합이 변하는 개방성(openness). 기존 논의를 확정하자면, BPO가 상태 가치 추정의 회피로 CTDE 비평자 문제를 우회했다면([[critic-free-optimization]]), TANDEM은 비평자를 유지하되 정보 조건을 실행 정합적으로 만드는 제2 경로로 '회피 vs 정합화' 스펙트럼의 양극과 그 사이 하이브리드 위치를 완성한다. SeeQ와의 상보성도 유지된다 — 가치 추정의 난제는 추정 자체가 아니라 입도(백업 지평)와 정보 조건의 결합 함수다. 개방성 차원은 [[non-stationary-dynamics]]의 극단 형태로, 환경 파라미터가 아니라 참여 주체 집합 자체가 변하면 학습된 정책의 정보 가정이 근본에서 무효화된다. 이는 수치 정합성 수준의 [[training-inference-mismatch]]와 동형이되 정책-정보 수준에서 발생하는 병리이며, 전역 정보로 국소 정합성을 학습한 정책이 실행 조건에서 전역 무효성으로 전환되는 구조를 제공한다.

## 🔗 관련 논문

- TANDEM: Balancing Centralized and Decentralized Critics to Address the Information Gap in Complex Multi-Agent Environments (2026-10-29)

## 🏷️ 엔티티

- [[entities/tandem-critics.md|tandem-critics]]
- [[entities/ctde-information-gap.md|ctde-information-gap]]
- [[entities/critic-free-optimization.md|critic-free-optimization]]
- [[entities/state-value-estimation-avoidance.md|state-value-estimation-avoidance]]
- [[entities/seeq.md|seeq]]
- [[entities/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[entities/imperfect-perception.md|imperfect-perception]]
- [[entities/training-inference-mismatch.md|training-inference-mismatch]]
- [[entities/local-coherence-global-incoherence.md|local-coherence-global-incoherence]]
- [[entities/multi-agent-reinforcement-learning.md|multi-agent-reinforcement-learning]]

## 📐 개념

- [[concepts/tandem-critics.md|tandem-critics]]
- [[concepts/ctde-information-gap.md|ctde-information-gap]]
- [[concepts/imperfect-perception.md|imperfect-perception]]
- [[concepts/training-inference-mismatch.md|training-inference-mismatch]]
- [[concepts/information-usability-gap.md|information-usability-gap]]
- [[concepts/openness.md|openness]]

---
_LLM 분석으로 생성됨_
