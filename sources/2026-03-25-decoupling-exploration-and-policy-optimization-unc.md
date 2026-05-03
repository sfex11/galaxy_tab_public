# Decoupling Exploration and Policy Optimization: Uncertainty Guided Tree Search for Hard Exploration

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22273v1

## 💡 핵심 인사이트

탐색과 정책 최적화를 분리하고 불확실성 기반 트리 탐색으로 탐색을 수행함으로써, 내재적 보상 합성의 간섭 문제를 구조적으로 해소하는 새로운 RL 패러다임을 제시한다.

## 📖 분석

## Decoupling Exploration and Policy Optimization: Uncertainty Guided Tree Search for Hard Exploration

본 논문은 강화학습(RL)에서 탐색(exploration)과 정책 최적화(policy optimization)를 분리(decoupling)하는 새로운 패러다임을 제안한다. 기존 접근법은 내재적 보상(intrinsic reward)과 외재적 보상(extrinsic reward)을 합성한 복합 목적함수를 최적화하는 방식으로 탐색 문제를 해결해왔으나, 이는 두 목표 간의 간섭으로 인해 불필요한 오버헤드를 발생시킨다. 저자들은 정책 최적화가 정밀한 과제 수행에는 필수적이지만, 탐색 자체에는 반드시 필요하지 않다고 주장한다.

핵심 방법론은 **불확실성 기반 트리 탐색(Uncertainty Guided Tree Search)**으로, 에이전트의 불확실성 추정을 활용하여 탐색 방향을 결정하는 트리 기반 계획 알고리즘이다. 이를 통해 탐색 단계에서는 RL 정책 업데이트 없이도 효율적으로 유용한 데이터를 수집하고, 수집된 데이터로 별도의 정책 최적화를 수행한다.

이 접근법은 기존 강화학습의 탐색-활용(exploration-exploitation) 트레이드오프 문제를 구조적으로 재정의한다는 점에서 의의가 있다. 특히 하드 탐색(hard exploration) 문제—보상이 희소하거나 환경이 복잡한 경우—에서 기존 내재적 동기 기반 방법들의 한계를 극복할 수 있는 가능성을 보여준다. 트리 탐색과 불확실성 추정의 결합은 모델 기반 RL 및 계획(planning) 연구와도 밀접한 관련이 있다.

## 🔗 관련 논문

- 2026 04 10 android coach improve online agentic training effi
- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 09 in place test time training

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/transfer-learning.md|transfer-learning]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/gpu-kernel-optimization.md|gpu kernel optimization]]

---
**관련**: [[concepts/bilevel-optimization.md|bilevel optimization]]

---
**관련**: [[concepts/myopic-optimization.md|myopic optimization]]

---
**관련**: [[entities/solver-poser-decoupling.md|solver poser decoupling]]
