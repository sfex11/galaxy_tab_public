# Planning in entropy-regularized Markov decision processes and games

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-23
**링크**: http://arxiv.org/abs/2604.19695v1

## 💡 핵심 인사이트

엔트로피 정규화가 벨만 연산자에 부여하는 smoothness가 비정규화 MDP에서는 다항식 샘플 복잡도 보장이 전혀 존재하지 않는 상황에서 문제 독립적 O~(1/ε⁴) 계획을 가능하게 하며, 정규화는 계산적 가능성 자체를 역전시키는 구조적 메커니즘이다.

## 📖 분석

# SmoothCruiser: 엔트로피 정규화 MDP·게임에서의 계획

## 정의
SmoothCruiser는 엔트로피 정규화된 마르코프 결정 과정(MDP) 및 2인 게임에서 생성 모델(generative model)을 기반으로 가치 함수를 추정하는 계획 알고리즘이다.

## 기존 Wiki와의 관계

### reinforcement-learning: 정규화가 계산적 가능성을 역전시키는 사례
기존 RL 합성 분석에서 강조된 "현실 세계에서 작동하는 RL"이라는 메타 주제와 연결된다. 비정규화 설정에서는 다항식 샘플 복잡도를 보장하는 알고리즘이 존재하지 않는데, 엔트로피 정규화 하나의 추가로 문제 독립적 O~(1/ε⁴) 보장이 달성된다는 발견은 [[concepts/exploration-absorption-decoupling.md|탐색-흡수 분리]] 패러다임과 맞닿아 있다: 정규화가 탐색 경로를 부드럽게 만들어 표본 효율성의 비약적 개선을 가능하게 한다는 점에서, RL의 기여를 "경로 제공자"로 재정의하는 기존 개념을 강화한다.

### markov-decision-process: 벨만 연산자의 매끄러움(smoothness)이라는 새 축
기존 MDP 개념에 벨만 연산자의 smoothness라는 분석 차원을 추가한다. 엔트로피 정규화가 부여하는 Lipschitz 연속성이 샘플 복잡도의 기하급수적-다항식 경계를 결정짓는 핵심 인자임을 수학적으로 입증한다.

### stochastic-optimal-control: 게임 확장
기존 density-driven optimal control 논문들이 단일 에이전트 설정을 다루었다면, SmoothCruiser는 2인 게임으로 확장하여 다중 에이전트 최적 제어와의 연결점을 제공한다.

## 다른 논문과의 연결점
- [[sources/2026-04-06-model-based-reinforcement-learning-for-control-und.md|GP 기반 MBRL]]: 생성 모델 기반이라는 공통점이 있으나, SmoothCruiser는 비정상성 가정 없이 문제 독립적 보장을 제공한다는 차별점.
- [[sources/2026-04-12-density-driven-optimal-control-convergence-guarant.md|Density-Driven Optimal Control]]: 수렴 보장에 대한 이론적 관심을 공유하나, 엔트로피 정규화라는 다른 메커니즘 사용.

## 🔗 관련 논문

- 2026-04-06-model-based-reinforcement-learning-for-control-und
- 2026-04-12-density-driven-optimal-control-convergence-guarant
- 2026-04-13-density-driven-optimal-control-convergence-guarant

## 🏷️ 엔티티

- [[entities/markov-decision-process.md|markov-decision-process]]
- [[entities/reinforcement-learning.md|reinforcement-learning]]

## 📐 개념

- [[concepts/entropy-regularized-planning.md|entropy-regularized-planning]]
- [[concepts/smooth-bellman-operator.md|smooth-bellman-operator]]
- [[concepts/generative-model-planning.md|generative-model-planning]]
- [[concepts/sample-complexity-guarantee.md|sample-complexity-guarantee]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[concepts/invariance-entropy.md|invariance entropy]]
