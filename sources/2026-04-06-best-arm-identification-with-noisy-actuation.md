# Best-Arm Identification with Noisy Actuation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02255v1

## 💡 핵심 인사이트

MAB의 최적 팔 식별 문제에서 actuation noise를 DMC로 모델링하면, 샘플 복잡도가 채널의 영-오류 용량(zero-error capacity)에 의해 결정된다는 정보 이론적 연결을 최초로 규명했다.

## 📖 분석

## Best-Arm Identification with Noisy Actuation

본 논문은 **다중 팔 밴딧(Multi-Armed Bandit, MAB)** 문제에서 최적 팔(best arm)을 식별하는 과제를, 중앙 학습자(central learner)와 분산 에이전트(distributed agent) 간 통신 채널에 노이즈가 존재하는 상황으로 확장한다. 핵심적으로, 팔 선택 명령이 **이산 무기억 채널(Discrete Memoryless Channel, DMC)**을 통해 전달될 때 발생하는 actuation noise를 다루며, 에이전트의 능력(capabilities)에 따라 서로 다른 통신 방식(communication scheme)을 설계하고 분석한다.

### 핵심 기여

이 연구의 독창성은 MAB의 탐색(exploration) 문제를 **정보 이론적 관점**에서 재구성한 데 있다. 최적 팔 식별의 샘플 복잡도가 기저 DMC의 **영-오류 용량(zero-error capacity)**과 밀접하게 연결된다는 점을 보인다. 이는 전통적 밴딧 알고리즘이 가정하는 '완벽한 행동 실행'을 넘어, 실제 분산 시스템에서의 통신 제약을 반영한다.

### 기존 Wiki와의 연결

- **분산 최적화(distributed-optimization)** 관점에서, 중앙-에이전트 구조의 통신 제약 하 의사결정 문제라는 점에서 ADMM 기반 분산 MPC 연구와 구조적 유사성이 있다.
- **다중 에이전트 시스템(multi-agent-system)**에서 에이전트 간 불완전한 통신이 의사결정 품질에 미치는 영향을 분석한다는 점에서, 분산 에이전트 협업 연구 흐름과 연결된다.
- **강화학습(reinforcement-learning)**의 탐색-활용 트레이드오프를 통신 이론으로 확장한 것으로, 기존 RL 기반 밴딧 연구의 가정을 근본적으로 재검토한다.
- **계산 복잡도(computational-complexity)** 측면에서, 적대적 환경에서의 최적 경로 계획 연구와 마찬가지로 이론적 하한(lower bound)과 달성 가능한 상한(upper bound)을 분석한다.

### 시사점

로봇 군집, IoT 센서 네트워크, 분산 LLM 에이전트 시스템 등 noisy 통신 환경에서의 최적 의사결정에 직접 적용 가능한 이론적 프레임워크를 제공한다.

## 🔗 관련 논문

- ADMM-Based Distributed MPC with Control Barrier Functions fo
- Density-Driven Optimal Control: Convergence Guarantees for S
- Optimal Path Planning in Hostile Environments
- Decoupling Exploration and Policy Optimization: Uncertainty

## 📐 개념

- [[concepts/multi-armed-bandit.md|multi-armed-bandit]]
- [[concepts/zero-error-capacity.md|zero-error-capacity]]
- [[concepts/noisy-actuation.md|noisy-actuation]]

---
_LLM 분석으로 재생성됨_
