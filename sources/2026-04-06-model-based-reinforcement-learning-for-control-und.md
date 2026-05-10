# Model-Based Reinforcement Learning for Control under Time-Varying Dynamics

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02260v1

## 💡 핵심 인사이트

비정상 동역학 환경에서 가우시안 프로세스 기반 연속적 모델 학습을 통해, 시스템 변화에 적응하는 강화학습 제어의 이론적 프레임워크를 제시한다.

## 📖 분석

## Model-Based Reinforcement Learning for Control under Time-Varying Dynamics

본 논문은 시스템 동역학이 시간에 따라 변화하는 비정상(non-stationary) 환경에서의 강화학습 제어 문제를 다룬다. 기존 학습 기반 제어 방법들이 정상(stationary) 동역학을 가정하는 것과 달리, 드리프트, 마모, 운영 조건 변화 등으로 인해 전이 동역학이 에피소드마다 진화하는 **연속적 모델 기반 강화학습(continual model-based RL)** 세팅을 제안한다. 가우시안 프로세스(GP) 동역학 모델을 활용하여 불확실성을 명시적으로 모델링하며, 변화하는 환경에 적응적으로 대응한다.

### 기존 Wiki와의 연결

**[[concepts/reinforcement-learning.md|reinforcement learning]]** 엔티티와 직접적으로 관련되며, 특히 모델 기반 접근법이라는 점에서 모델 프리 방법 중심의 기존 RL 논문들과 차별화된다. **[[concepts/distribution-shift.md|distribution shift]]** 개념과 밀접한데, 동역학 자체가 시간에 따라 변화하는 것이 분포 이동의 한 형태이다. **[[concepts/meta-learning.md|meta learning]]** 개념과도 연결되는데, 에피소드 간 빠른 적응이 핵심 과제이며, 'Unified Policy Value Decomposition for Rapid Adaptation' 논문의 빠른 적응 주제와 공명한다. 또한 **[[concepts/model-predictive-control.md|model predictive control]]** 개념과 관련이 깊으며, GP 기반 동역학 모델 위에서 제어 정책을 최적화하는 구조는 MPC 패러다임과 유사하다.

'Robust Quadruped Locomotion via Evolutionary RL'(2026-04-10)이 진화적 방법으로 로봇 제어의 강건성을 추구한 것과 비교하면, 본 논문은 모델 불확실성의 명시적 추적을 통해 적응성을 확보하는 상보적 접근을 취한다.

## 🔗 관련 논문

- Robust Quadruped Locomotion via Evolutionary Reinforcement Learning
- Unified Policy Value Decomposition for Rapid Adaptation
- Decoupling Exploration and Policy Optimization: Uncertainty
- Federated Distributional Reinforcement Learning with Distrib

## 📐 개념

- [[concepts/model-based-rl.md|model-based-rl]]
- [[concepts/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[concepts/gaussian-process-dynamics.md|gaussian-process-dynamics]]
- [[concepts/continual-learning.md|continual-learning]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/non-stationary-dynamics.md|non stationary dynamics]]

---
**관련**: [[entities/time-varying-confounding.md|time varying confounding]]

---
**관련**: [[concepts/experience-dynamics-extraction-gap.md|experience dynamics extraction gap]]
