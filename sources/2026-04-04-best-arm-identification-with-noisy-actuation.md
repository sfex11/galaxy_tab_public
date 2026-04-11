# Best-Arm Identification with Noisy Actuation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02255v1

## 💡 핵심 인사이트

최적 팔 식별 문제에서 통신 채널의 영-오류 용량이 탐색 효율의 근본적 한계를 결정하며, 이는 정보이론과 순차적 의사결정 이론의 새로운 연결고리를 제시한다.

## 📖 분석

## Best-Arm Identification with Noisy Actuation

본 논문은 **다중 팔 밴딧(Multi-Armed Bandit, MAB)** 문제에서 중앙 학습기(central learner)와 분산 에이전트(distributed agent) 사이의 팔 선택 명령이 **이산 무기억 채널(Discrete Memoryless Channel, DMC)**을 통해 전달될 때 최적 팔을 식별하는 문제를 다룬다. 기존 MAB 연구가 완벽한 명령 전달을 가정하는 것과 달리, 본 연구는 통신 잡음이 탐색 전략에 미치는 영향을 분석한다.

### 핵심 기여
- 에이전트의 능력(디코딩 가능 여부 등)에 따른 통신 방식(communication scheme)을 설계하고 분석
- 최적 팔 식별 성능이 DMC의 **영-오류 용량(zero-error capacity)**과 밀접하게 연결됨을 보임
- 정보이론과 순차적 의사결정(sequential decision-making)의 교차점에서 새로운 이론적 결과 제시

### Wiki 내 연결점
본 연구는 [[distributed-optimization]]과 개념적으로 연결된다. 분산 환경에서 중앙-에이전트 간 통신 제약 하에 최적화를 수행한다는 점에서 [[multi-agent-system]]의 통신 프로토콜 설계와도 관련이 있다. 또한 불확실성 하의 탐색-활용 균형이라는 면에서 [[reinforcement-learning]]의 탐색(exploration) 문제와 이론적 기반을 공유하며, [[decoupling-exploration-and-policy-optimization]] 논문의 탐색 전략 분리 아이디어와도 맥을 같이 한다. 정보이론적 하한(lower bound)을 활용하는 접근은 [[scaling-laws]] 연구에서 모델 성능의 이론적 한계를 규명하는 방법론과 유사한 분석 철학을 보인다.

## 🔗 관련 논문

- Decoupling Exploration and Policy Optimization: Uncertainty
- ADMM-Based Distributed MPC with Control Barrier Functions fo
- Density-Driven Optimal Control: Convergence Guarantees for S
- Federated Distributional Reinforcement Learning with Distrib

## 📐 개념

- [[concepts/multi-armed-bandit.md|multi-armed-bandit]]
- [[concepts/zero-error-capacity.md|zero-error-capacity]]
- [[concepts/noisy-communication.md|noisy-communication]]

---
_LLM 분석으로 재생성됨_
