# New LoRA Skills Should Read but Never Write

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31600v1

## 💡 핵심 인사이트

새 LoRA 스킬의 합성 성패는 병합 알고리즘의 정교함이 아니라 새 어댑터에 부여되는 읽기-쓰기 권한 구조가 결정하며, 새 스킬은 기존 계산을 읽기만 하고 절대 쓰지 않을 때만 기존 능력과 간섭 없이 공존한다.

## 📖 분석

### New LoRA Skills Should Read but Never Write (2026-09-29)

독립 훈련된 LoRA 어댑터들의 단일 모델 합성 실패(가중치 병합 간섭, 전체 재훈련 비용, 라우팅에 의한 단일 모델 목표 포기)를 모든 합성 방법이 암묵적으로 수행하는 두 선택 — 동치 인수분해의 선택과 읽기-쓰기 권한 구조 — 로 추적한다. LoRA 업데이트는 무한히 많은 동치 인수분해를 허용하므로, 어느 인수분해로 표현했는가가 간섭 여부를 결정한다.

핵심 원칙은 새 스킬 어댑터가 기존 계산을 '읽을' 수는 있되 다른 스킬이 의존하는 활성화·파라미터에는 '쓰지' 말아야 한다는 것이다. 이는 [[regression-tax]]의 파라미터 수준 기제와 구조적 예방책을 동시에 제공하며, [[monotonic-skill-benefit-assumption]]이 성립하는 조건(쓰기 권한의 부재)을 명시한다.

[[capability-internalization]]의 비용 구조를 규정한다 — 가중치로의 능력 이식은 기존 능력과의 쓰기 충돌을 회피하는 부분공간([[low-rank-adaptation-subspace]])에 국한될 때만 안전하다. [[skill-as-external-state]]의 외부 스킬 라우팅([[native-skill-routing]])과 대비되는 '가중치 내부 스킬'의 설계 제약을 확정하고, [[model-merging]]을 가중치 공간 산술에서 권한 구조 설계의 문제로 재정의한다.

## 🔗 관련 논문

- LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language 
- Merging the Knowledge of LLMs for Automatic Speech Recogniti
- Skill-Conditioned Gated Self-Distillation for LLM Reasoning
- The Router Within: Eliciting Native Skill Routing from a Fro
- Forgetting Only What Matters: Layer-Selective Unlearning tow

## 🏷️ 엔티티

- [[entities/low-rank-adaptation-subspace.md|low-rank-adaptation-subspace]]
- [[entities/capability-internalization.md|capability-internalization]]
- [[entities/model-merging.md|model-merging]]
- [[entities/skill-conditioned-gating.md|skill-conditioned-gating]]
- [[entities/skill-lifecycle-management.md|skill-lifecycle-management]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/lora-skill-composition.md|lora-skill-composition]]

## 📐 개념

- [[concepts/regression-tax.md|regression-tax]]
- [[concepts/monotonic-skill-benefit-assumption.md|monotonic-skill-benefit-assumption]]
- [[concepts/parameter-decoupling.md|parameter-decoupling]]
- [[concepts/read-only-skill-addition.md|read-only-skill-addition]]
- [[concepts/factorization-underdetermination.md|factorization-underdetermination]]

---
_LLM 분석으로 생성됨_
