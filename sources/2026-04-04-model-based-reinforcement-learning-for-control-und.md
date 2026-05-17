# Model-Based Reinforcement Learning for Control under Time-Varying Dynamics

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02260v1

## 💡 핵심 인사이트

비정상(non-stationary) 동역학 환경에서 가우시안 프로세스 기반 모델을 활용한 연속적 MBRL 프레임워크가 정상성 가정 없이도 적응적 제어를 가능하게 한다.

## 📖 분석

## Model-Based Reinforcement Learning for Control under Time-Varying Dynamics

본 논문은 시스템 동역학이 시간에 따라 변화하는 환경에서의 강화학습 제어 문제를 다룬다. 기존 학습 기반 제어 방법들이 정상(stationary) 동역학을 가정하는 것과 달리, 드리프트, 마모, 운영 조건 변화 등으로 인해 전이 동역학이 에피소드마다 진화하는 **연속적 모델 기반 강화학습(continual MBRL)** 세팅을 제안한다. 가우시안 프로세스(GP) 동역학 모델을 활용하여 비정상 환경에서의 적응적 제어를 분석한다.

### 기존 Wiki와의 연결

[[concepts/reinforcement-learning.md|reinforcement learning]] 엔티티의 핵심 확장 연구로, 정상성 가정을 완화한 점이 차별점이다. [[concepts/distribution-shift.md|distribution shift]] 개념과 직접 연관되며, 동역학 변화를 분포 이동(distribution shift)의 일종으로 볼 수 있다. [[concepts/meta-learning.md|meta learning]] 개념과도 연결되는데, 에피소드마다 변하는 환경에 빠르게 적응하는 능력이 메타학습의 핵심 목표와 일치한다. [[concepts/world-model.md|world model]] 개념에서 GP 기반 동역학 모델은 환경의 월드 모델을 명시적으로 학습하는 접근법에 해당한다.

기존 소스 중 robust quadruped locomotion 연구가 진화적 강화학습으로 로봇 제어의 강건성을 다룬 점에서 상보적이며, federated distributional RL 연구도 분산 환경에서의 RL 일반화 문제를 공유한다.

## 🔗 관련 논문

- Robust Quadruped Locomotion via Evolutionary Reinforcement Learning
- Federated Distributional Reinforcement Learning with Distributed
- Decoupling Exploration and Policy Optimization: Uncertainty
- Unified Policy Value Decomposition for Rapid Adaptation

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/distribution-shift.md|distribution-shift]]
- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/world-model.md|world-model]]
- [[concepts/model-predictive-control.md|model-predictive-control]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/time-varying-confounding.md|time varying confounding]]
