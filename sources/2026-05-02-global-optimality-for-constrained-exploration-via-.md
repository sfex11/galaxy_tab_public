# Global Optimality for Constrained Exploration via Penalty Regularization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-02
**링크**: http://arxiv.org/abs/2604.28144v1

## 💡 핵심 인사이트

엔트로피 최대화의 비가산성 구조가 벨만 방정식 기반 분해를 근본적으로 불가능하게 하며, 페널티 정규화가 이 장벽을 우회하여 제약 탐색의 전역 최적성을 보장한다.

## 📖 분석

# Constrained Exploration via Penalty Regularization

강화학습에서 탐색(exploration)은 종종 상태-행동 점유측(occupancy measure)의 엔트로피 최대화로 공식화된다. 그러나 기존 엔트로피 정규화 연구([[sources/2026-04-23-planning-in-entropy-regularized-markov-decision-pr.md|엔트로피 정규화 MDP 계획]])는 **비제약(unconstrained)** 설정을 전제로 하며, 실세계 탐색은 안전성·자원·모방 제약을 동반한다.

이 논문은 제약 탐색이 근본적으로 더 어려운 **구조적 이유**를 최초로 명시한다: 엔트로피 최대화는 가산성(additive) 구조를 갖지 않아, [[entities/markov-decision-process|MDP]]의 벨만 방정식 기반 분해가 불가능하다. 이는 [[concepts/entropy-regularized-planning|엔트로피 정규화 계획]]이 제약 설정으로 자연스럽게 확장될 수 없음을 의미한다.

제안된 페널티 정규화(penalty regularization)는 이 비가산성 장벽을 우회하여 **전역 최적성(global optimality)**을 달성하는 경로를 제공한다. 기존 [[concepts/safety-aware-exploration|안전 인지 탐색]]이 GP 기반 경험적 접근이었다면, 본 논문은 제약 탐색의 형식적 기반을 제공하여 [[concepts/safety-critical-control|안전 임계 제어]]와 탐색 이론 사이의 간극을 메운다.

## 🔗 관련 논문

- 2026 04 23 planning in entropy regularized markov decision pr
- 2026 04 24 a hough transform approach to safety aware scalar f
- 2026 05 01 safe navigation using neural radiance fields via r

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]
- [[entities/safety-aware-exploration.md|safety-aware-exploration]]
- [[entities/entropy-regularized-planning.md|entropy-regularized-planning]]

## 📐 개념

- [[concepts/constrained-exploration.md|constrained-exploration]]
- [[concepts/penalty-regularization.md|penalty-regularization]]
- [[concepts/occupancy-measure-optimization.md|occupancy-measure-optimization]]
- [[concepts/non-additive-exploration.md|non-additive-exploration]]

---
_LLM 분석으로 생성됨_
