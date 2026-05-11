# Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-11
**링크**: http://arxiv.org/abs/2605.06650v1

## 💡 핵심 인사이트

GRPO가 단순화한 advantage 추정을 위해 도입한 음성 롤아웃이 검증 불가능한 출력의 노이즈를 흡수 과정에 주입하여, training-process-gaming과 구조적으로 동일한 패턴의 문제를 야기한다 — POPO의 암묵적 음성 기울기는 검증 불가능한 출력에서 기울기를 생성하지 않는다는 점에서 노이즈 원천을 구조적으로 차단한다.

## 📖 분석

# Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients (2026-05-11)

RLVR(검증 가능 보상 기반 강화학습) 패러다임에서 PPO에서 GRPO로의 전환은 advantage 추정의 복잡도를 줄인 것으로 평가받아왔다. 그러나 본 논문은 GRPO가 양성/음성 롤아웃 기반 단순 추정이 실제로는 **검증 불가능한 음성 롤아웃의 노이즈가 흡수 과정을 오염시켜 training-process-gaming과 구조적으로 유사한 문제**를 야기한다고 지적한다.

핵심 기여는 세 가지로 정리된다. 첫째, negative-rollout-noise의 구체적 메커니즘을 제공한다 — 검증 불가능한 음성 출력에서 도출된 기울기가 근본적으로 신뢰할 수 없는 반면, 이것이 GRPO의 advantage 분산을 인위적으로 팽창시킨다. 둘째, positive-only-policy-optimization의 실제 메커니즘을 정의한다 — 양성 롤아웃만 사용하면서 검증 결과(정답/오답)를 implicit-negative-gradient로 변환하여 보상 차이를 재구성하는 방식. 셋째, 이것이 exploration-absorption-decoupling에 미치는 영향을 구조화한다 — 음성 롤아웃의 노이즈가 흡수 채널을 오염시키므로, 탐색 경로의 품질을 보존하면서 능력으로 전이하는 분리의 근본 전제가 훼손됨을 보인다.

openvlthinkerv2가 GRPO 기반으로 학습된 모델이라는 점에서, POPO가 직접 적용 가능한 주요 타겟이 되며, GRPO의 노이즈 문제가 이 모델의 학습 효율에 미친 영향을 재평가할 수 있는 실증 무대가 된다. 또한 template-constrained-decoding이 외부 제약으로 출력 공간을 제한하는 방식과 대비되는 내부 보상 구조 기반 정제 경로를 제공한다.

## 🔗 관련 논문

- OpenVLThinkerV2: A Generalist Multimodal Reasoning Model for
- Crafting Reversible SFT Behaviors in Large Language Models
- Exploration Hacking: Can LLMs Learn to Resist RL Training?

## 🏷️ 엔티티

- [[entities/positive-only-policy-optimization.md|positive-only-policy-optimization]]
- [[entities/negative-rollout-noise.md|negative-rollout-noise]]
- [[entities/implicit-negative-gradient.md|implicit-negative-gradient]]
- [[entities/grpo.md|grpo]]
- [[entities/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]
- [[entities/false-positive-convergence.md|false-positive-convergence]]
- [[entities/exploration-avoidance-tradeoff.md|exploration-avoidance-tradeoff]]

## 📐 개념

- [[concepts/implicit-negative-gradient.md|implicit-negative-gradient]]
- [[concepts/negative-rollout-noise.md|negative-rollout-noise]]

---
_LLM 분석으로 생성됨_
