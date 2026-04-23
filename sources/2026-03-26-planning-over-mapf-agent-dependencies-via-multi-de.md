# Planning over MAPF Agent Dependencies via Multi-Dependency PIBT

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23405v1

## 💡 핵심 인사이트

PIBT의 단일 충돌 제약을 다중 의존성 그래프로 확장함으로써, 대규모 혼잡 환경에서 MAPF의 효율성과 해 품질을 동시에 개선할 수 있다.

## 📖 분석

## Planning over MAPF Agent Dependencies via Multi-Dependency PIBT

본 논문은 Multi-Agent Path Finding(MAPF) 문제에서 널리 사용되는 Priority Inheritance with Backtracking(PIBT) 알고리즘의 근본적 한계를 분석하고 이를 극복하는 Multi-Dependency PIBT(MD-PIBT)를 제안한다.

### 문제 인식
PIBT는 수백~수천 에이전트가 혼잡한 환경에서 실시간으로 경로를 계획할 수 있는 효율적인 알고리즘이지만, 규칙 기반 계획 절차에 의해 제약되며 **최대 하나의 다른 에이전트와 충돌하는 경로만 탐색**할 수 있다는 구조적 한계를 갖는다. 이는 복잡한 다중 에이전트 의존성(multi-dependency)이 존재하는 상황에서 최적 해를 찾지 못하는 원인이 된다.

### 핵심 기여
MD-PIBT는 에이전트 간 의존성 그래프를 명시적으로 모델링하여, 단일 충돌 제약을 넘어 **다중 에이전트 의존성을 동시에 고려한 계획**을 수행한다. 이를 통해 PIBT의 효율성을 유지하면서도 탐색 공간을 확장하여 더 일반적인 해를 도출할 수 있다.

### 연구 맥락
기존 Wiki의 [[concepts/multi-agent-path-planning.md|multi agent path planning]] 개념과 직접적으로 연결되며, ADMM 기반 분산 MPC나 Density-Driven Optimal Control 등 다중 에이전트 조율 연구와 문제 도메인을 공유한다. 특히 [[concepts/multi-robot-coordination.md|multi robot coordination]]에서 다루는 충돌 회피 및 협조적 계획 문제의 구체적 알고리즘 개선 사례에 해당한다. 또한 [[concepts/computational-complexity.md|computational complexity]]와 관련하여, 대규모 에이전트 환경에서의 계산 효율성과 해의 품질 간 트레이드오프를 다룬다.

## 🔗 관련 논문

- Optimal Path Planning in Hostile Environments
- ADMM-Based Distributed MPC with Control Barrier Functions fo
- Density-Driven Optimal Control: Convergence Guarantees for S
- CAMO: A Conditional Neural Solver for the Multi-objective Mu

## 📐 개념

- [[concepts/multi-agent-path-planning.md|multi-agent-path-planning]]
- [[concepts/computational-complexity.md|computational-complexity]]
- [[concepts/multi-robot-coordination.md|multi-robot-coordination]]

---
_LLM 분석으로 재생성됨_
