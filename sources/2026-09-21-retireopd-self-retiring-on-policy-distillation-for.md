# RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20784v1

## 💡 핵심 인사이트

교사 감독은 단계 조건부 자원이며 특권 정보조차 교사 신뢰성을 담보하지 않으므로, 증류 체계는 교사의 자발적 퇴역을 설계 요소로 내장해야 한다.

## 📖 분석

# RetireOPD: Self-Retiring On-Policy Distillation for Agentic RL

멀티턴 에이전트 RL이 궤적당 단일 스칼라 보상만 받는다는 진단([[reward-sparsity]], [[trajectory-level-objective]])에서 출발해, 특권적 태스크 스킬을 가진 셀프 교사가 밀집 토큰 수준 감독을 공급하고 무스킬 학생이 이를 내재화하는 셀프 온폴리시 증류([[on-policy-self-distillation]]) 계열의 후속 연구다. 본 논문은 두 실증 발견으로 이 레시피를 보정한다. (1) 특권 정보만으로 교사가 신뢰 가능해지지 않는다([[privileged-reliability-decoupling]]) — 스킬 보유가 올바른 지도를 담보하지 않는다. (2) 교사 감독의 이익은 훈련 단계에 의존한다([[stage-dependent-teacher-supervision]]) — 초반의 가속이 후기에는 학생의 자율 탐색을 방해하는 부하로 역전된다. 이에 따라 교사가 자신의 한계 이익을 판정해 스스로 퇴역하는 셀프 리타이어드 메커니즘을 제안한다([[self-retiring-distillation]]).

## 기존 Wiki와의 관계

OPD의 길이 부풀림 안정화(Demystifying OPD, 2026-04)와 Flow-OPD가 증류의 '품질' 문제를 다뤘다면, 본 논문은 증류의 '수명' 문제를 연다. 단계 의존성은 [[sft-rl-budget-allocation]]을 정적 배분에서 시간축 동적 재배분으로 전환시키며, 교사 퇴역 이후의 후기 학습 경로는 [[teacher-free-step-compression]]과 접속된다. 특권-신뢰성 분리는 expertise≠judgment 구조의 증류 도메인 확립이며, [[skill-conditioned-gating]]의 스킬 조건부 게이팅과 달리 '언제 게이트를 내릴 것인가'를 다룬다. Learning to Coach의 코치-액터 분리([[coach-actor-decoupling]])에 '코치의 퇴역' 차원을 더해 감독자 생애주기 설계라는 새 축을 형성한다.

## 🔗 관련 논문

- Demystifying OPD: Length Inflation and Stabilization Strateg
- Flow-OPD: On-Policy Distillation for Flow Matching Models
- Cliff: Learning Process Rewards from the First Mistake
- Learning to Coach for Experiential Learning
- Skill-Conditioned Gated Self-Distillation for LLM Reasoning

## 🏷️ 엔티티

- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/self-retiring-distillation.md|self-retiring-distillation]]
- [[entities/stage-dependent-teacher-supervision.md|stage-dependent-teacher-supervision]]
- [[entities/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]
- [[entities/reward-sparsity.md|reward-sparsity]]
- [[entities/sft-rl-budget-allocation.md|sft-rl-budget-allocation]]

## 📐 개념

- [[concepts/on-policy-self-distillation.md|on-policy-self-distillation]]
- [[concepts/trajectory-level-objective.md|trajectory-level-objective]]
- [[concepts/turn-level-credit-estimation.md|turn-level-credit-estimation]]
- [[concepts/teacher-free-step-compression.md|teacher-free-step-compression]]
- [[concepts/coach-actor-decoupling.md|coach-actor-decoupling]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]

---
_LLM 분석으로 생성됨_
