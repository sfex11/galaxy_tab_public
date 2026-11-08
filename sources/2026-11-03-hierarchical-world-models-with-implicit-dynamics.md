# Hierarchical World Models with Implicit Dynamics

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42146v1

## 💡 핵심 인사이트

장기 과제 세계 모델 플래닝의 병목은 동역학 예측 오차 자체보다 도달가능성과 동역학의 결합에 있으며, 이 결합을 계층 간 기능 분해로 분리하는 것이 매크로 액션의 경직성 없이 누적 오차와 탐색 복잡도를 동시에 완화한다.

## 📖 분석

ID-WM(Implicit Dynamics World Models)은 상태 공간 도달가능성과 동역학을 분리하는 world-model로, 장기 과제의 누적 오차([[concepts/compounding-error.md|compounding error]])와 탐색 복잡도를 완화한다. 매크로 액션·잠재 스킬 기반 기존 계층화가 취약한 표현과 제한된 정밀 제어를 낳는다는 진단은, stage-transition-learning가 밝힌 '계층적 플래닝의 최약 고리 = 전이 판정'과 상통하며 [[concepts/hierarchical-planning.md|hierarchical planning]]의 경계 설계 문제를 표현 문제로 재정의한다.

world-model 논의에 두 갈래 기여를 제공한다. 첫째, [[concepts/world-model-in-pieces.md|world model in pieces]]가 빅월드 체제에서 등변적 단일 잠재 동역학([[concepts/faithful-latent-world-model.md|faithful latent world model]])의 획득이 구조적으로 어렵다고 보였다면, ID-WM은 도달가능성 구조를 동역학에서 분리해 계층별 표현 요구를 달리 함으로써 단일 통합 동역학의 부담을 우회하는 아키텍처적 응답을 제시한다. 둘째, [[concepts/transition-lookahead-planning.md|transition lookahead planning]]이 형식화한 접근-계획 간극의 아키텍처 실현으로, 도달가능성이 상위 계층의 1급 대상이 됨을 보여준다. 이는 [[concepts/reachable-set.md|reachable set]]이 안전 분석 도구로 다루던 도달가능성이 플래닝 추상화로 확장됨을 의미하며, 세계 모델 플래닝이 [[concepts/test-time-scaling.md|test time scaling]]의 체화 도메인 실현임도 재확인한다. 신규 개념 reachability-dynamics-decoupling과 implicit-dynamics의 위키 등재가 필요하다.

## 🔗 관련 논문

- Understanding the limits of latent world models
- Near-Optimal Reinforcement Learning with Multi-Step Transition Lookahead
- StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks
- SeeQ: Training Generalist Value Functions for Long-Horizon Robotic Manipulation
- Benchmarking World Models for Continual Learning on Compositional Tasks

## 🏷️ 엔티티

- [[entities/id-wm.md|id-wm]]
- [[entities/world-model.md|world-model]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/compounding-error.md|compounding-error]]

## 📐 개념

- [[concepts/reachability-dynamics-decoupling.md|reachability-dynamics-decoupling]]
- [[concepts/implicit-dynamics.md|implicit-dynamics]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[entities/meta-learning.md|meta learning]]

---
**관련**: [[concepts/controllable-opinion-dynamics.md|controllable opinion dynamics]]

---
**관련**: [[concepts/completion-learning-separation.md|completion learning separation]]

---
**관련**: [[concepts/functional-learning-criterion.md|functional learning criterion]]

---
**관련**: [[concepts/quantization-error-accumulation.md|quantization error accumulation]]

---
**관련**: [[concepts/interdependent-movement-planning.md|interdependent movement planning]]

---
**관련**: [[concepts/self-reinforcing-verification-error-orbit.md|self reinforcing verification error orbit]]

---
**관련**: [[concepts/dynamic-task-composition.md|dynamic task composition]]

---
**관련**: [[concepts/execution-record-as-learning-corpus.md|execution record as learning corpus]]

---
**관련**: [[concepts/planning-mode-declaration.md|planning mode declaration]]

---
**관련**: [[concepts/delegation-scope-dynamic-governance.md|delegation scope dynamic governance]]

---
**관련**: [[concepts/reproduction-work-compounding.md|reproduction work compounding]]
