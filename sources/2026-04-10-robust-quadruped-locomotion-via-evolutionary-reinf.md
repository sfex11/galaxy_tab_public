# Robust Quadruped Locomotion via Evolutionary Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07224v1

## 💡 핵심 인사이트

진화적 탐색(CEM)과 기울기 기반 강화학습(DDPG/TD3)의 결합이 단일 정책 최적화 대비 환경 변화에 대한 로버스트니스를 개선할 수 있으며, 이는 sim-to-real 전이의 핵심 병목을 해소하는 실용적 방향을 제시한다.

## 📖 분석

## Robust Quadruped Locomotion via Evolutionary Reinforcement Learning

본 논문은 시뮬레이션에서 훈련된 사족보행 정책이 환경 변화 시 전이에 실패하는 문제를 다루며, **진화적 강화학습(Evolutionary Reinforcement Learning)**을 통해 이를 해결하고자 한다. DDPG, TD3, 그리고 Cross-Entropy Method(CEM)을 결합한 CEM-DDPG, CEM-TD3 네 가지 방법을 평면 지형 보행 과제에서 비교 평가한다.

### 핵심 접근법

기울기 기반 정책 최적화(gradient-based policy optimisation)와 **집단 기반 탐색(population-driven exploration)**을 결합하는 것이 핵심이다. CEM 변형은 정책 파라미터 공간에서 진화적 탐색을 수행하면서 동시에 RL의 샘플 효율성을 활용한다. 이는 단일 정책 최적화가 빠지기 쉬운 국소 최적점(local optima)을 회피하고, 환경 변화에 대한 **로버스트니스**를 확보하는 데 기여한다.

### 기존 Wiki와의 연결

이 연구는 [[reinforcement-learning]] 엔티티 및 개념과 직접적으로 연관된다. 특히 [[distribution-shift]] 문제를 sim-to-real 전이 관점에서 다루며, [[model-based-rl]]과 대비되는 model-free 접근법의 로버스트니스를 탐구한다. 또한 로봇 보행이라는 도메인에서 [[embodied-ai]]와 연결되며, 진화 알고리즘의 활용은 [[metaheuristic-optimization]]의 연장선에 있다. CEM의 집단 기반 탐색은 [[self-organizing-systems]]의 원리와도 맞닿아 있다.

사족보행 로봇의 sim-to-real 전이 문제는 [[autonomous-driving]]의 closed-loop 평가([[closed-loop-evaluation]])에서 다루는 시뮬레이션-현실 간극 문제와 구조적으로 유사하다.

## 🔗 관련 논문

- Robust Quadruped Locomotion via Evolutionary Reinforcement Learning
- Model-Based Reinforcement Learning for Control under Time-Va
- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- Decoupling Exploration and Policy Optimization: Uncertainty
- Specification-Aware Distribution Shaping for Robotics Founda

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/distribution-shift.md|distribution-shift]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/metaheuristic-optimization.md|metaheuristic-optimization]]
- [[concepts/closed-loop-evaluation.md|closed-loop-evaluation]]

---
_LLM 분석으로 재생성됨_
