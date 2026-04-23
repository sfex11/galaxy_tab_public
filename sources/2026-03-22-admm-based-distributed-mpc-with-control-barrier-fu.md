# ADMM-Based Distributed MPC with Control Barrier Functions for Safe Multi-Robot Quadrupedal Locomotion

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19170v1

## 💡 핵심 인사이트

CBF 제약이 도입하는 에이전트 간 커플링을 ADMM 분산 최적화로 분해함으로써, 다중 사족보행 로봇의 안전성 보장과 계산 확장성을 동시에 달성한다.

## 📖 분석

## ADMM-Based Distributed MPC with Control Barrier Functions for Safe Multi-Robot Quadrupedal Locomotion

본 논문은 다중 로봇 사족보행 시스템의 안전-임계(safety-critical) 궤적 계획을 위한 완전 분산형 모델 예측 제어(MPC) 프레임워크를 제안한다. 핵심 기여는 제어 장벽 함수(Control Barrier Function, CBF) 제약 조건을 MPC에 통합하여 에이전트 간 충돌 회피를 보장하면서도, ADMM(Alternating Direction Method of Multipliers) 기반 분산 최적화를 통해 중앙 집중식 계산의 병목을 해소한 점이다.

CBF 제약은 에이전트 간 명시적 커플링을 도입하여 최적 제어 문제의 직접 분해를 불가능하게 만드는데, 저자들은 이를 구조화된 분산 최적화 프레임워크로 재정식화하여 해결한다. 각 로봇이 자신의 로컬 MPC 문제만 풀면서도 전체 시스템의 안전성을 보장하는 구조이다.

이 연구는 [[concepts/reinforcement-learning.md|강화학습]] 기반 사족보행 제어와 상호보완적 관계에 있다. 강화학습이 단일 로봇의 적응적 보행 정책을 학습하는 데 강점을 보이는 반면, 본 연구의 MPC+CBF 접근은 다중 로봇 환경에서 형식적 안전성 보장을 제공한다. 특히 [[concepts/convex-optimization.md|볼록 최적화]] 이론을 활용한 ADMM 분해는 분산 시스템의 확장성 문제를 해결하는 핵심 도구로 작용한다.

[[concepts/multi-agent-system.md|다중 에이전트 시스템]] 관점에서, CBF 기반 안전 제약의 분산 처리는 에이전트 간 통신 오버헤드를 최소화하면서 안전성을 유지하는 실용적 방법론을 제시한다.

## 🔗 관련 논문

- Robust Quadruped Locomotion via Evolutionary Reinforcement Learning

## 📐 개념

- [[concepts/control-barrier-function.md|control-barrier-function]]
- [[concepts/model-predictive-control.md|model-predictive-control]]
- [[concepts/distributed-optimization.md|distributed-optimization]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/safety-critical-control.md|safety critical control]]

---
**관련**: [[concepts/safety-critical-control.md|safety critical control]]

---
**관련**: [[concepts/memory-as-control-resource.md|memory as control resource]]

---
**관련**: [[concepts/function-vector.md|function vector]]

---
**관련**: [[concepts/inventory-control.md|inventory control]]

---
**관련**: [[concepts/heterogeneous-robot-team.md|heterogeneous robot team]]

---
**관련**: [[concepts/density-driven-optimal-control.md|density driven optimal control]]

---
**관련**: [[concepts/training-inference-process-control-continuum.md|training inference process control continuum]]

---
**관련**: [[concepts/stochastic-optimal-control.md|stochastic optimal control]]

---
**관련**: [[concepts/sampled-data-control.md|sampled data control]]
