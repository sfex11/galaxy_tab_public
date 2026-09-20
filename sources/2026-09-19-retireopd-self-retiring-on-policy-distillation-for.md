# RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20784v1

## 💡 핵심 인사이트

교사 감독의 이득은 훈련 단계에 의존하고 특권 정보는 교사 신뢰성을 보장하지 않으므로, 밀집 감독은 상시 구성요소가 아니라 스스로 은퇴하는 임시 스캐폴드로 설계되어야 한다.

## 📖 분석

RetireOPD는 다중 턴 에이전트 RL에서 궤적당 단일 스칼라 보상이라는 희소성([[concepts/reward-sparsity.md|reward sparsity]], [[concepts/trajectory-level-objective.md|trajectory level objective]])을 보완하기 위해 특권 태스크 스킬을 가진 셀프-교사가 토큰 수준 밀집 감독을 공급하는 self-OPD를 검토하되, 두 발견으로 무조건적 채택을 거부한다: 특권 정보가 교사의 신뢰성을 보장하지 않으며, 교사 감독의 이득은 훈련 단계 의존적이다. 이에 따라 증류를 영구 구성요소가 아닌 유익한 단계가 끝나면 스스로 은퇴하는 임시 스캐폴드로 설계한다.

이는 [[concepts/on-policy-distillation.md|on policy distillation]]의 상시성 전제에 대한 구조적 수정이다. [[entities/nemotron-cascade-2.md|nemotron cascade 2]] 계열의 cascade RL이 증류를 파이프라인 단계로 구성했다면([[concepts/cascade-reinforcement-learning.md|cascade reinforcement learning]]), RetireOPD는 그 단계의 종료 조건을 명시적 설계 대상으로 삼아 '언제까지 증류할 것인가'라는 스케줄링 질문을 추가한다. [[concepts/process-reward-model.md|process reward model]]과 달리 외부 검증기 없이 셀프-교사로 밀집 감독을 실현하는 대안 경로이며, [[concepts/teacher-free-step-compression.md|teacher free step compression]]이 처음부터 교사 없이 설계했다면 교사 보유→은퇴→교사 없음의 동적 전이 경로를 제공한다. [[concepts/sft-rl-budget-allocation.md|sft rl budget allocation]]의 관점에서도 감독과 순수 RL 간 예산을 고정이 아닌 단계 조건부 동적 배분으로 확장한다.

핵심 시사: 밀집 감독에도 한계 효용의 소멸이 존재하므로, 감독 기제 자체에 종료 조건이 필요하다.

## 🔗 관련 논문

- 2026-03-23-nemotron-cascade-2-post-training-llms-with-cascade
- 2026-04-12-demystifying-opd-length-inflation-and-stabilizatio
- 2026-09-16-discrete-beckmann-transport-models-for-one-step-la
- 2026-09-16-bellman-policy-optimization
- 2026-05-12-flow-opd-on-policy-distillation-for-flow-matching-

## 🏷️ 엔티티

- [[entities/retireopd.md|retireopd]]

## 📐 개념

- [[concepts/on-policy-distillation.md|on-policy-distillation]]
- [[concepts/cascade-reinforcement-learning.md|cascade-reinforcement-learning]]
- [[concepts/on-policy-self-distillation.md|on-policy-self-distillation]]
- [[concepts/reward-sparsity.md|reward-sparsity]]
- [[concepts/trajectory-level-objective.md|trajectory-level-objective]]
- [[concepts/process-reward-model.md|process-reward-model]]
- [[concepts/teacher-free-step-compression.md|teacher-free-step-compression]]
- [[concepts/sft-rl-budget-allocation.md|sft-rl-budget-allocation]]
- [[concepts/turn-level-credit-estimation.md|turn-level-credit-estimation]]
- [[concepts/self-retiring-distillation.md|self-retiring-distillation]]
- [[concepts/stage-dependent-teacher-supervision.md|stage-dependent-teacher-supervision]]
- [[concepts/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]

---
_LLM 분석으로 생성됨_
