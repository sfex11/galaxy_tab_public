# Score Centering Stabilizes Off-policy Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20807v1

## 💡 핵심 인사이트

RL 불안정성의 근원은 TIM 자체가 아니라 매 학습 스텝 누적되는 drift이며, 스코어 센터링이라는 알고리즘 측 보정만으로 롤아웃 효율을 희생하지 않고 오프폴리시 RL을 안정화할 수 있다.

## 📖 분석

# Score Centering Stabilizes Off-policy Reinforcement Learning

## 핵심 진단: 불안정의 원인은 TIM 자체가 아니라 drift

LLM RL이 훈련-추론 불일치(TIM)에 극도로 민감하다는 것은 기지의 사실이지만, TIM 완전 제거는 롤아웃 효율에 막대한 비용을 요구해 비실용적이다. 본 논문은 불안정의 진짜 원인을 **drift** — 매 학습 스텝마다 누적되는 훈련-추론 엔진 간의 지속적 편향 — 로 특정하고, 스코어 센터링이 이 편향을 제거하여 안정화를 달성함을 보인다.

## Wiki 관계망에서의 위치

**[[negative-rollout-noise]]와의 병인 대칭**: 음성 롤아웃 노이즈는 모델-환경 상호작용의 우연적 오염(처방: 노이즈 배제, POPO)이고, TIM drift는 인프라 차이의 계통적 편향(처방: 편향 중심화)이다. 학습 신호 오염 연구가 '우연 vs 계통' 두 병인 축으로 분해 완성된다.

**[[training-inference-mismatch]]의 원인 분해**: 문제는 수치 불일치 그 자체가 아니라 그것이 시간축 위에서 누적되는 방식([[cumulative-drift]])이며, TIM 대응 목표가 '제로 불일치'에서 'drift 제거'로 재정의된다.

**알고리즘-인프라 쌍방 흡수**: TIM 흡수가 인프라 측(수치 일치)과 알고리즘 측(수학적 보정) 양쪽에서 가능함을 실증한다. [[on-policyness-as-infrastructure-guarantee]]가 온폴리시성의 인프라 조건화를 주장했다면, 본 논문은 알고리즘 보정이 동일 안정성을 달성하는 보완 축임을 보여준다. 오프폴리시 RL이 drift 제거 조건 하에서 안정화되면 [[retireopd]]의 온폴리시 증류와 대비되는 효율적 대안 경로가 열린다.

## 🔗 관련 논문

- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning

## 🏷️ 엔티티

- [[entities/score-centering.md|score-centering]]
- [[entities/training-inference-mismatch.md|training-inference-mismatch]]
- [[entities/cumulative-drift.md|cumulative-drift]]
- [[entities/negative-rollout-noise.md|negative-rollout-noise]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/retireopd.md|retireopd]]

## 📐 개념

- [[concepts/bias-noise-decoupling.md|bias-noise-decoupling]]
- [[concepts/rollout-efficiency-exactness-tradeoff.md|rollout-efficiency-exactness-tradeoff]]
- [[concepts/systemic-engine-drift.md|systemic-engine-drift]]
- [[concepts/on-policyness-as-infrastructure-guarantee.md|on-policyness-as-infrastructure-guarantee]]
- [[concepts/mismatch-algorithm-bidirectional-absorption.md|mismatch-algorithm-bidirectional-absorption]]

---
_LLM 분석으로 생성됨_
