# ADMM-Based Distributed MPC with Control Barrier Functions for Safe Multi-Robot Quadrupedal Locomotion

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19170v1

## 💡 핵심 인사이트

CBF 제약이 유발하는 에이전트 간 결합 문제를 ADMM 분산 최적화로 분해함으로써, 중앙 제어 없이도 다중 4족 로봇의 수학적 안전성 보장이 가능함을 보인 점이 핵심이다.

## 📖 분석

## ADMM-Based Distributed MPC with Control Barrier Functions for Safe Multi-Robot Quadrupedal Locomotion

본 논문은 다중 로봇 4족 보행 시스템의 안전-임계(safety-critical) 궤적 계획을 위한 완전 분산형 모델 예측 제어(MPC) 프레임워크를 제안한다. 핵심 기여는 제어 장벽 함수(Control Barrier Function, CBF) 제약 조건을 MPC에 통합하되, 에이전트 간 결합(inter-agent coupling) 문제를 ADMM(Alternating Direction Method of Multipliers) 기반 분산 최적화로 해결한 점이다.

### 핵심 구조
- **CBF 제약**: 로봇 간 충돌 회피를 위한 명시적 안전 제약으로, 에이전트 간 상태 결합을 유발
- **ADMM 분해**: 중앙집중식 문제를 각 로봇이 독립적으로 풀 수 있는 부분 문제로 분해
- **분산 MPC**: 각 로봇이 로컬 계산만으로 전역 안전성을 보장하는 궤적 생성

### 기존 연구와의 관계
본 연구는 [[concepts/reinforcement-learning.md|reinforcement learning]] 기반 4족 보행 제어와 상보적 관계에 있다. RL이 단일 로봇의 적응적 보행 정책을 학습하는 데 강점을 보이는 반면, 본 프레임워크는 다중 로봇 간 안전 보장이라는 수학적 증명 가능한 속성에 초점을 맞춘다. 특히 'Robust Quadruped Locomotion via Evolutionary RL' 논문이 진화적 RL로 단일 4족 로봇의 강건성을 다룬 반면, 본 논문은 다중 로봇 협조 문제로 범위를 확장한다.

[[concepts/convex-optimization.md|convex optimization]] 관점에서 ADMM은 볼록 분해 기법의 대표적 방법론이며, 기존 Wiki의 'A Convex Formulation of the Multi-Commodity Dynamic Traffic Assignment' 논문과 분산 최적화라는 방법론적 공통점을 공유한다. 또한 [[concepts/multi-agent-system.md|multi agent system]] 개념과 직접 연결되며, 안전 제약 하 다중 에이전트 협조라는 새로운 각도를 제공한다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 09 social dynamics as critical vulnerabilities that u

## 📐 개념

- [[concepts/control-barrier-function.md|control-barrier-function]]
- [[concepts/model-predictive-control.md|model-predictive-control]]
- [[concepts/distributed-optimization.md|distributed-optimization]]
- [[concepts/multi-robot-coordination.md|multi-robot-coordination]]

---
_LLM 분석으로 재생성됨_
