# Bellman Policy Optimization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15987v1

## 💡 핵심 인사이트

자회귀 생성의 종단 보상 설정에서 Bellman 방정식을 통한 궤적 수준 재구성이 중간 상태 가치 추정 없이도 PMD와 동일한 유일 최적해를 달성함을 증명하여, LLM RLVR에서 크리틱 계층의 이론적 불필요성을 확립한다.

## 📖 분석

# Bellman Policy Optimization (BPO)

## 정의

RLVR(검증 가능 보상 강화학습)의 추론 능력 향상을 위한 크리틱 프리(critic-free) 방법으로, Policy Mirror Descent(PMD)에서 유도된다. 자회귀 생성 + 종단 보상 설정에서 Bellman 방정식을 이용해 PMD를 궤적 수준 목적함수로 재구성하며, 이 재구성이 중간 상태의 가치 추정을 완전히 회피하면서도 기존 형식과 동일한 유일 최적해를 가짐을 증명한다.

## 기존 Wiki와의 관계

- **[[concepts/rlvr.md|rlvr]]**: Wiki의 RLVR 논의([[concepts/grpo.md|grpo]], [[concepts/positive-only-policy-optimization.md|positive only policy optimization]])는 크리틱 프리 설계를 경험적 휴리스틱으로 채택해왔다. BPO는 동일한 설계가 PMD 이론에서 자연스럽게 유도됨을 보여 이론적 정당화를 제공한다.
- **[[concepts/relative-credit-assignment.md|relative credit assignment]]**: 중간 상태 가치 추정 없이도 종단 보상이 궤적 분포에 반영될 수 있음을 증명하여, 크레딧 할당 문제를 '추정 문제'에서 'Bellman 재구성 문제'로 전환한다.
- **[[concepts/entropy-regularized-planning.md|entropy regularized planning]]**: 엔트로피 정규화 MDP 계획 이론이 LLM 사후학습으로 이전되는 직접 사례로, 이론-실무 연속성을 확립한다.
- **[[concepts/reward-sparsity.md|reward sparsity]]**: 종단(희소) 보상이 궤적 수준 재구성의 적용 조건이라는 점에서, 희소성이 병목이 아니라 크리틱 제거의 근거가 될 수 있음을 시사한다.

## Wiki 관점의 의의

RL 이론([[concepts/transition-lookahead-planning.md|transition lookahead planning]] 계열)과 사후학습 실무([[concepts/grpo.md|grpo]]) 사이의 결측 간선 — 'LLM 자회귀 생성을 MDP로 형식화할 때 이론적으로 최소인 최적화 구조는 무엇인가' — 를 채운다. 사후학습 방법의 평가 축이 성능 비교에서 최적해 동등성 증명으로 확장될 수 있음을 제안한다.

## 🔗 관련 논문

- Near-Optimal Reinforcement Learning with Multi-Step Transition Lookahead
- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients
- Cliff: Learning Process Rewards from the First Mistake
- Planning in entropy-regularized Markov decision processes
- Post-Training Language Models for Gold-Medal Performance in Coding Competitions

## 🏷️ 엔티티

- [[entities/bellman-policy-optimization.md|bellman-policy-optimization]]
- [[entities/policy-mirror-descent.md|policy-mirror-descent]]
- [[entities/critic-free-optimization.md|critic-free-optimization]]
- [[entities/trajectory-level-objective.md|trajectory-level-objective]]
- [[entities/rlvr.md|rlvr]]
- [[entities/grpo.md|grpo]]
- [[entities/relative-credit-assignment.md|relative-credit-assignment]]
- [[entities/entropy-regularized-planning.md|entropy-regularized-planning]]
- [[entities/reward-sparsity.md|reward-sparsity]]
- [[entities/post-training.md|post-training]]

## 📐 개념

- [[concepts/bellman-equation-reformulation.md|bellman-equation-reformulation]]
- [[concepts/terminal-reward-only-learning.md|terminal-reward-only-learning]]
- [[concepts/state-value-estimation-avoidance.md|state-value-estimation-avoidance]]
- [[concepts/mirror-descent-optimization.md|mirror-descent-optimization]]
- [[concepts/unique-optimal-solution-guarantee.md|unique-optimal-solution-guarantee]]

---
_LLM 분석으로 생성됨_
