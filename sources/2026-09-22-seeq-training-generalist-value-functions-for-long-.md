# SeeQ: Training Generalist Value Functions for Long-Horizon Robotic Manipulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22085v1

## 💡 핵심 인사이트

장기 과제의 가치 학습 실패는 구조적 불가능이 아니라 추정 입도의 문제이며, 서브태스크 단위 가치 추정이 희소 보상·긴 크레딧 지평·벨만 백업 난이도를 동시에 완화한다.

## 📖 분석

SeeQ는 범용 로봇 정책이 다단계·장기 조작 과제에서 취약한 근인을 — 희소 태스크 수준 보상이 낳는 긴 크레딧 할당 지평, 어려운 벨만 백업, 광범위한 데이터 커버리지 요구 — 로 진단하고, 서브태스크 수준 Q-가치 함수로 해결한다. 가치 함수가 후보 행동의 순위화와 정책 개선 유도에 배치되며, 가치 추정 입도를 태스크에서 서브태스크로 낮추는 것이 핵심 설계다.

[[stage-transition-learning]]과의 관계가 중심이다. StageGuard([[stageguard]])가 '언제 단계를 전환할까'를 학습했다면 SeeQ는 '각 단계가 얼마나 잘 진행되는가'를 가치로 추정한다. 경계 판단과 진행도 평가는 장기 구조 학습의 상보적 두 축으로, 결합 시 학습된 전이 계층 위에 학습된 단계별 가치가 얹히는 스택이 성립하며 [[skill-termination-judgment]]은 종료 판단 근거를 가치 수렴으로 삼는 경로를 얻는다.

[[bellman-policy-optimization]]의 [[state-value-estimation-avoidance]]와 대조를 이룬다. BPO가 상태 가치 추정을 회피했다면 SeeQ는 백업 지평을 단축해 가치 추정을 실현 가능하게 한다 — 가치 추정의 어려움이 구조적 불가능이 아니라 입도 문제임을 시사하며, [[discount-regime-hardness]]가 규명한 장기 지평 체제 난이도의 실용적 완화다.

[[credit-assignment-granularity]] 관점에서 서브태스크 가치는 태스크-행동 사이 중간 입도를 제공하는 로보틱스 구현이며, [[reward-sparsity]] 완화의 알고리즘 측 경로다. [[on-policy-distillation]] 계열이 밀집 교사 신호로 희소성을 완화한 것과 달리 가치 추정 입도 조정으로 같은 문제를 푼다. [[hierarchical-planning]]에는 전이 판정과 진행도 가치가 모두 학습 대상이 되는 계층의 학습화 흐름을, [[end-to-end-vla-training]]에는 VLA 개선이 외부 가치 신호와 결합하는 계층을 부여한다.

## 🔗 관련 논문

- StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning
- Near-Optimal Reinforcement Learning with Multi-Step Transition Lookahead
- OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Free Teacher

## 🏷️ 엔티티

- [[entities/seeq.md|seeq]]
- [[entities/stageguard.md|stageguard]]
- [[entities/stage-transition-learning.md|stage-transition-learning]]
- [[entities/skill-termination-judgment.md|skill-termination-judgment]]
- [[entities/credit-assignment-granularity.md|credit-assignment-granularity]]
- [[entities/reward-sparsity.md|reward-sparsity]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/bellman-policy-optimization.md|bellman-policy-optimization]]
- [[entities/state-value-estimation-avoidance.md|state-value-estimation-avoidance]]
- [[entities/discount-regime-hardness.md|discount-regime-hardness]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/markov-decision-process.md|markov-decision-process]]
- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]

## 📐 개념

- [[concepts/subtask-level-value-function.md|subtask-level-value-function]]
- [[concepts/value-function-as-action-ranker.md|value-function-as-action-ranker]]
- [[concepts/generalist-value-function.md|generalist-value-function]]

---
_LLM 분석으로 생성됨_
