# Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06650v1

## 💡 핵심 인사이트

음성 롤아웃을 실제 생성하지 않고 암묵적 미분으로 그 기울기 기여를 합성함으로써, RLVR에서 탐색 비용과 노이즈를 동시에 제거하는 제3의 최적화 경로를 개척한다.

## 📖 분석

# Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients

## RLVR 패러다임에서 부정 샘플의 문제 진단

검증 가능 보상 기반 강화학습(RLVR)이 LLM 추론 능력 강화의 지배적 패러다임으로 자리 잡으면서, PPO에서 GRPO로의 빠른 전환이 일어났다. GRPO는 복잡한 어드밴티지 추정을 양성·음성 롤아웃의 단순 그룹 비교로 대체했으나, 본 논문은 **음성 롤아웃이 도입하는 노이즈가 최적화 안정성을 저해한다**는 문제를 체계적으로 진단한다. 이는 기존 Wiki에서 탐색-흡수 분리([[exploration-absorption-decoupling]])가 암묵적으로 전제하던 '탐색 경로의 품질이 균일하다'는 가정을 해체한다.

## 암묵적 부정 기울기의 명시적 대체

핵심 기여는 양성 샘플만으로도 부정 샘플의 기울기 기여를 **암묵적 미분(implicit differentiation)**으로 계산하는 Positive-Only Policy Optimization (POPO)를 제안한 것이다. 이는 [[distribution-internal-optimization]]의 새로운 구현 경로가 된다 — 부정 샘플을 외부에서 생성하여 분포 외부 탐색하는 것이 아니라, 양성 분포 내부에서 암묵적으로 부정 방향의 기울기를 합성한다. [[template-constrained-decoding]]이 분포 내부 출력 공간을 구조적으로 축소했다면, POPO는 분포 내부에서 부정 방향을 합성하여 탐색 비용 자체를 제거한다.

## 훈련 과정 게이밍과의 연결

[[exploration-hacking]]이 모델이 탐색 분포를 전략적으로 조작하는 문제라면, POPO는 **탐색 공간 자체를 축소**함으로써 게이밍의 공격 표면을 구조적으로 제한한다. 음성 롤아웃 생성이 불필요하므로, [[false-positive-convergence]]의 위험(쉬운 궤적만 탐색하여 위양성 수렴)도 완화된다. [[training-process-gaming]]의 해법 스펙트럼에서, 출력 제어(reward hacking) → 탐색 제어(exploration hacking) → 탐색 공간 제거(POPO)로 이어지는 점진적 제어 강화의 연속성을 제공한다.

## GRPO 생태계에의 영향

[[grpo]]를 사용하는 [[openvlthinkerv2]] 등 다수 모델에 직접적 영향을 미친다. POPO는 GRPO의 단순성을 유지하면서 노이즈 원천을 제거하므로, [[exploration-avoidance-tradeoff]]에서 '탐색 회피'가 아닌 '탐색 불필요'라는 제3의 해법 축을 연다.

## 🔗 관련 논문

- 2026 04 12 openvlthinkerv2 a generalist multimodal reasoning model for
- 2026 05 02 exploration hacking can llms learn to resist rl tr
- 2026 05 03 global optimality for constrained exploration via penalty re
- 2026 05 02 reliable answers for recurring questions boosting text to s

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]
- [[entities/post-training.md|post-training]]
- [[entities/grpo.md|grpo]]
- [[entities/exploration-hacking.md|exploration-hacking]]
- [[entities/exploration-absorption-decoupling.md|exploration-absorption-decoupling]]
- [[entities/distribution-internal-optimization.md|distribution-internal-optimization]]
- [[entities/training-process-gaming.md|training-process-gaming]]
- [[entities/false-positive-convergence.md|false-positive-convergence]]
- [[entities/exploration-avoidance-tradeoff.md|exploration-avoidance-tradeoff]]
- [[entities/openvlthinkerv2.md|openvlthinkerv2]]
- [[entities/template-constrained-decoding.md|template-constrained-decoding]]
- [[entities/positive-only-policy-optimization.md|positive-only-policy-optimization]]

## 📐 개념

- [[concepts/positive-only-policy-optimization.md|positive-only-policy-optimization]]
- [[concepts/implicit-negative-gradient.md|implicit-negative-gradient]]
- [[concepts/rlvr.md|rlvr]]
- [[concepts/negative-rollout-noise.md|negative-rollout-noise]]

---
_LLM 분석으로 생성됨_
