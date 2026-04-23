# A Hough transform approach to safety-aware scalar field mapping using Gaussian Processes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20799v1

## 💡 핵심 인사이트

안전 임계치를 가우시안 프로세스 추론의 구조적 제약으로 내재화하고 Hough 변환으로 위험 경계를 추정함으로써, '물리적 제약 미인코딩 계획' 문제를 확률적 모델 수준에서 해결하는 안전 인식 탐사 패러다임을 제시한다.

## 📖 분석

# 안전 인식 스칼라 필드 매핑: Hough 변환과 가우시안 프로세스의 융합

이 논문은 미지의 스칼라 필드(방사선, 화학 농도, 온도 등)를 고위험 환경에서 안전하게 매핑하기 위한 프레임워크를 제안한다. 핵심 아이디어는 스칼라 필드를 가우시안 프로세스(GP)로 모델링하되, 안전 임계치를 초과하는 고강도 영역을 회피하면서 효율적으로 탐사하는 데 있다.

## 기존 Wiki와의 관계

이 논문은 기존 Wiki의 여러 연구 축을 물리적 안전 문제로 수렴시킨다. **SafetyALFRED**가 체화 에이전트의 안전 계획 평가 부재를 지적했다면, 본 논문은 그 결함에 대한 정량적 해법을 제시한다 — 안전 임계치를 GP 추론의 구조적 제약으로 내재화하여, **물리적 제약 미인코딩 계획** 문제를 확률적 모델 수준에서 해결한다.

**Control Barrier Function** 기반 MPC 연구들이 안전 집합(safe set)을 동역학적 제약으로 정의했다면, 본 논문은 이를 정적 스칼라 필드의 공간적 제약으로 확장한다. Hough 변환을 안전 경계 탐지에 활용하는 점은 [[concepts/computational-geometry.md|computational geometry]]과 [[concepts/autonomous-driving-perception.md|autonomous driving perception]]에서의 기하학적 접근을 위험 영역 식별로 전이한 사례다.

## 주요 기여

GP의 불확실성 추정과 안전 임계치를 결합하여 탐사 경로를 생성하는 방식은, 기존 **area-coverage** 문제에 안전 제약을 부가한 확장이다. [[concepts/density-driven-optimal-control.md|density driven optimal control]]이 밀도 기반 커버리지 보장을 다뤘다면, 본 논문은 불균일한 위험 분포 하에서의 커버리지를 다룬다.

[[concepts/model-based-rl.md|model based rl]]과 [[concepts/gaussian-process-dynamics.md|gaussian process dynamics]]이 시변 동역학의 GP 모델링에 집중했다면, 본 논문은 정적 필드의 공간적 GP 모델링을 안전 제약과 결합하여, GP의 활용 범위를 시간 영역에서 공간 영역으로 확장한다.

## 🔗 관련 논문

- 2026-04-23-safetyalfred-evaluating-safety-conscious-planning-.md
- 2026-04-12-density-driven-optimal-control-convergence-guarant.md
- 2026-04-06-model-based-reinforcement-learning-for-control-und.md
- 2026-04-07-minimal-information-control-invariance-via-vector-.md
- 2026-03-22-admm-based-distributed-mpc-with-control-barrier-fu.md

## 🏷️ 엔티티

- [[entities/gaussian-process-dynamics.md|gaussian-process-dynamics]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/ai-safety.md|ai-safety]]
- [[entities/area-coverage.md|area-coverage]]
- [[entities/safety-critical-control.md|safety-critical-control]]

## 📐 개념

- [[concepts/scalar-field-mapping.md|scalar-field-mapping]]
- [[concepts/hough-transform.md|hough-transform]]
- [[concepts/safety-aware-exploration.md|safety-aware-exploration]]
- [[concepts/safety-threshold-gp-constraint.md|safety-threshold-gp-constraint]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[concepts/gaussian-splatting.md|gaussian splatting]]
