# CAMO: A Conditional Neural Solver for the Multi-objective Multiple Traveling Salesman Problem

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19074v1

## 💡 핵심 인사이트

단일 조건부 신경망으로 다중 에이전트 조율과 다목적 트레이드오프를 동시에 해결하여, 기존에 분리되어 있던 경로 최적화와 작업 분배 문제를 통합적으로 다룰 수 있음을 보였다.

## 📖 분석

## CAMO: 다목적 다중 외판원 문제를 위한 조건부 신경 솔버

CAMO(Conditional Approach for Multi-Objective optimization)는 다목적 다중 외판원 문제(MOMTSP)를 해결하기 위한 학습 기반 신경 솔버이다. 로봇 팀이 여러 목표 지점을 방문하면서 총 이동 비용과 최대 완료 시간(makespan) 같은 상충하는 목적함수를 동시에 최적화해야 하는 상황을 다룬다.

### 핵심 문제

MOMTSP는 단일 에이전트 TSP의 NP-hard 복잡도에 다중 에이전트 조율과 다목적 트레이드오프라는 이중 난제가 결합된 문제다. 기존 학습 기반 방법들은 단일 에이전트 TSP나 단일 목적 변형에서 강한 성능을 보였으나, 이 두 가지 도전을 동시에 다루는 연구는 드물었다.

### 기술적 접근

CAMO는 조건부 신경망 구조를 채택하여, 주어진 선호도 벡터(preference vector)에 따라 파레토 최적 해를 조건부로 생성한다. 이를 통해 단일 모델로 다양한 목적함수 간 트레이드오프를 탐색할 수 있으며, 다중 로봇 간 작업 분배와 경로 계획을 통합적으로 수행한다.

### 연구적 의의

이 연구는 [[convex-optimization|볼록 최적화]]와 [[reinforcement-learning|강화학습]] 분야의 교차점에 위치한다. 특히 다중 에이전트 경로 계획 문제에 신경 조합 최적화(neural combinatorial optimization)를 적용한 점에서, [[multi-agent-system|다중 에이전트 시스템]] 연구와 직접적으로 연결된다. 또한 로봇 시스템의 실시간 의사결정이라는 맥락에서 [[embodied-ai|체화된 AI]] 연구와도 관련성을 갖는다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf

## 📐 개념

- [[concepts/neural-combinatorial-optimization.md|neural-combinatorial-optimization]]
- [[concepts/multi-objective-optimization.md|multi-objective-optimization]]
- [[concepts/traveling-salesman-problem.md|traveling-salesman-problem]]

---
_LLM 분석으로 재생성됨_
