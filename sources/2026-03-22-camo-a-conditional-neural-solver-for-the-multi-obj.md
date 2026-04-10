# CAMO: A Conditional Neural Solver for the Multi-objective Multiple Traveling Salesman Problem

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19074v1

## 💡 핵심 인사이트

다중 에이전트 조율과 다목적 트레이드오프를 동시에 해결하는 조건부 신경 솔버를 제시하여, 신경 조합 최적화 분야를 단일 에이전트·단일 목적에서 다중 에이전트·다목적 설정으로 확장했다.

## 📖 분석

## CAMO: 다목적 다중 외판원 문제를 위한 조건부 신경 솔버

CAMO(Conditional Multi-Objective solver)는 다목적 다중 외판원 문제(MOMTSP)를 해결하기 위한 학습 기반 신경 솔버이다. 로봇 시스템에서 여러 에이전트가 다수의 목표 지점을 방문하면서 총 이동 비용(total travel cost)과 최대 완료 시간(makespan)이라는 상충하는 목적을 동시에 최적화해야 하는 문제를 다룬다.

### 핵심 기여

기존 학습 기반 방법들은 단일 에이전트 TSP나 다목적 TSP 변형에서 강력한 성능을 보였지만, **다중 에이전트 조율(multi-agent coordination)**과 **다목적 트레이드오프(multi-objective trade-offs)**를 동시에 다루는 경우는 드물었다. CAMO는 이 두 가지 도전을 결합하여 해결하는 조건부 신경 솔버로, 선호도 벡터를 조건으로 입력받아 다양한 파레토 최적 해를 단일 모델로 생성할 수 있다.

### 기존 Wiki와의 연결

이 연구는 **convex-optimization** 개념과 밀접한 관련이 있다. 다목적 최적화에서 파레토 프론티어 탐색은 볼록 최적화의 핵심 주제이며, 동적 교통 배정 문제([[convex-optimization]])와 유사한 조합 최적화 구조를 공유한다. 또한 **multi-agent-system** 엔티티와 직접적으로 연결되는데, 다중 로봇 협업 경로 계획이라는 점에서 에이전트 간 작업 분배와 조율 메커니즘을 다룬다. **reinforcement-learning** 개념과도 관련이 있으며, 신경 조합 최적화 솔버들이 강화학습 기반 훈련을 활용하는 추세와 맥을 같이 한다.

### 의의

신경 조합 최적화(Neural Combinatorial Optimization) 분야에서 다목적·다중 에이전트 설정을 동시에 처리하는 통합 프레임워크를 제시함으로써, 실제 로보틱스 응용에서의 경로 계획 문제 해결에 실질적 기여를 한다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/convex-optimization.md|convex-optimization]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_
