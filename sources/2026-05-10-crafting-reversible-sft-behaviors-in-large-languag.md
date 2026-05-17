# Crafting Reversible SFT Behaviors in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06632v1

## 💡 핵심 인사이트

SFT 유도 행동의 문제는 행동 자체가 아니라 그 행동이 모델 내부에 구조적 제약 없이 분포되어 인과적으로 비가역적이라는 점이며, 행동을 가역적으로 설계하는 것이 선택적 제어의 전제조건이다.

## 📖 분석

# Reversible SFT: SFT 유도 행동의 인과적 가역성 공학

기존 SFT(Supervised Fine-Tuning)는 모델에 새로운 행동을 유도하지만, 그 행동이 모델 내부에 어떤 구조적 제약을 가지고 분포하는지에 대한 규범이 없다. 기존의 회로 귀인(circuit attribution) 방식은 SFT 유도 행동과 상관된 희소 서브네트워크를 사후적으로 식별하지만, 상관관계가 인과적 필연성을 의미하지 않아 추론 시점에서 SFT 행동을 선택적으로 제어할 수 없다는 근본적 한계를 지적한다.

본 논문은 SFT 유도 행동을 **가역적(reversible)**으로 만드는 대안적 경로를 제시한다 — 즉, SFT 행동이 모델의 기존 능력과 얽혀 있지 않고, 식별된 회로에 인과적으로 필연적으로 분포되도록 SFT를 설계함으로써 추론 시 선택적 활성화/비활성화가 가능하게 한다. 이는 [[concepts/mechanistic-interpretability.md|기계적 해석가능성]]의 목표를 '상관적 식별'에서 '인과적 공학'으로 전환시키며, [[concepts/post-training.md|사후학습]] 패러다임이 가진 구조적 무제약(structural unconstrainedness) 문제를 최초로 형식화한다.

[[concepts/sft-hallucination-mechanism.md|SFT 환각 메커니즘]] 연구가 SFT가 어떤 특징을 활성화하는지를 관찰했다면, 본 논문은 그 특징이 **인과적 필연성을 갖도록 행동을 설계하는 방법**을 다룬다. [[concepts/exploration-absorption-decoupling.md|탐색-흡수 분리]]에서 RL이 경로를 제공하고 SFT가 흡수한다는 모델과 연결되면, 가역적 SFT는 흡수 과정 자체를 인과적으로 분리 가능하게 만드는 상위 제약이 된다. [[concepts/causal-mechanistic-interpretability.md|인과적 기계적 해석가능성]] 엔티티가 MoRFI 이후 제시했던 '개입 가능한 인과 경로 식별'이라는 목표에 대한 구체적 공학적 달성 경로를 제공한다.

## 🔗 관련 논문

- 2026-05-01-morfi-monotonic-sparse-autoencoder-feature-identif.md
- 2026-05-02-exploration-hacking-can-llms-learn-to-resist-rl-tr.md
- 2026-05-06-standing-on-the-shoulders-of-giants-stabilized-kno.md

## 🏷️ 엔티티

- [[entities/reversible-sft.md|reversible-sft]]
- [[entities/post-hoc-causal-gap.md|post-hoc-causal-gap]]
- [[entities/post-training.md|post-training]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/sft-hallucination-mechanism.md|sft-hallucination-mechanism]]
- [[entities/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]

## 📐 개념

- [[concepts/post-hoc-causal-gap.md|post-hoc-causal-gap]]
- [[concepts/reversible-behavior-engineering.md|reversible-behavior-engineering]]
- [[concepts/structural-behavior-unconstrainedness.md|structural-behavior-unconstrainedness]]
- [[concepts/causal-necessity-vs-correlation.md|causal-necessity-vs-correlation]]
- [[concepts/inference-time-behavior-control.md|inference-time-behavior-control]]

---
_LLM 분석으로 생성됨_
