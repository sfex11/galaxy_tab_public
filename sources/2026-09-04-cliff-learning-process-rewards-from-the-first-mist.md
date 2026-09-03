# Cliff: Learning Process Rewards from the First Mistake

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02817v1

## 💡 핵심 인사이트

롤아웃에서 첫 번째 실수가 발생하는 지점이 가장 정보가 풍부한 훈련 신호이며, 결과 보상을 그 클리프 지점을 기준으로 분해하면 전문화된 보상 모델이나 교사-학생 동질성 가정 없이도 프로세스 수준 가이드를 획득할 수 있다.

## 📖 분석

Cliff는 RLVR(검증 가능 보상 기반 강화학습)의 구조적 한계—거친 결과 보상이 중간 추론 과정에 가이드를 주지 못하는 문제—를, 전문화된 프로세스 보상 모델(PRM)이나 교사-학생 동일 추론 패턴 가정 없이 해결하는 경로를 제시한다. 핵심은 '첫 번째 실수(first mistake)'를 프로세스 보상의 앵커로 삼는 것이다: 롤아웃에서 첫 실수가 발생하는 클리프 지점을 탐지하고, 그 이전 prefix는 최종 성공에서 긍정 신호를, 이후 suffix는 부정 신호를 상속하도록 크레딧을 분해한다. 이는 unrecoverable-reasoning-error의 진단적 통찰—오류 이후 모든 토큰이 복합화된다는 것—을 훈련 신호 설계로 전환한 것으로, 오류 지점 자체가 최대 정보를 담는 앵커가 됨을 보여준다. 기존 [[rlvr]]이 purely-reactive-optimization에 머물렀던 것과 달리 프로세스 수준 신호를 자체 유도하며, 'Reconciling Process Supervision with Outcome-Based Rewards'(2026-09-02)가 다룬 프로세스-결과 보상 갈등에 대한 제3의 경로를 제공한다. 또한 [[on-policy-distillation]]의 교사-학생 동질성 가정을 벗어나 검증기만으로 프로세스 신호를 도출하므로, 'Scaling Large Reasoning Models beyond Human Supervision'(2026-09-03)과 함께 인간 감독 의존을 낮추는 보상 설계 축을 형성한다.

## 🔗 관련 논문

- Reconciling Process Supervision with Outcome Based Rewards (2026-09-02)
- Scaling Large Reasoning Models beyond Human Supervision (2026-09-03)
- Learning to Evaluate Before Improving Automatic Rubric Generation (2026-09-02)
- The Rise of Verbal Reinforcement Learning (2026-09-03)

## 🏷️ 엔티티

- [[entities/rlvr.md|rlvr]]
- [[entities/post-training.md|post-training]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]

## 📐 개념

- [[concepts/first-mistake-anchoring.md|first-mistake-anchoring]]
- [[concepts/process-reward-model.md|process-reward-model]]
- [[concepts/step-wise-verification-reward.md|step-wise-verification-reward]]
- [[concepts/relative-credit-assignment.md|relative-credit-assignment]]
- [[concepts/purely-reactive-optimization.md|purely-reactive-optimization]]
- [[concepts/reward-signal-substitution-failure.md|reward-signal-substitution-failure]]
- [[concepts/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[concepts/verifier-mediated-goal-delegation.md|verifier-mediated-goal-delegation]]
- [[concepts/credit-assignment-granularity.md|credit-assignment-granularity]]

---
_LLM 분석으로 생성됨_
