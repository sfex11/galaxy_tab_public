# Forgetting Only What Matters: Layer-Selective Unlearning toward Robust LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10439v1

## 💡 핵심 인사이트

언러닝으로 제거된 지식조차 양자화 같은 배포 변환 하에서 부활할 수 있으므로, 지식 제거의 보장은 모델 변환 불변량이 아니라 특정 배포 구성에 스코프된 조건부 상태다.

## 📖 분석

본 논문은 LLM이 민감·저작권·유해 콘텐츠를 기억하는 문제에서, 광범위·고정 파라미터 업데이트 방식의 언러닝이 유틸리티를 저하시키고 배포 변화에 취약함을 지적하며 레이어 선택적 언러닝을 제안한다.

위키 관점의 두 기여가 있다. 첫째, 망각 택소노미의 파라미터 축을 완성한다. 기존 위키의 망각 논의([[adaptive-forgetting]], [[selective-forgetting-as-safety]])는 에이전트 메모리·환경 잔재 수준이었으나, 본 논문은 가중치에 내재된 기억의 제거라는 파라미터 수준 망각을 추가한다. 둘째, 언러닝 보장의 구성 의존성을 실증한다 — 포스트 트레이닝 양자화가 제거된 지식을 부분 부활시켜, 제거 보장이 모델 변환 불변량이 아니라 배포 구성에 스코프된 조건부 상태임을 시사한다.

레이어 선택성은 [[model-pruning]]·[[layer-dropout]]과 '능력과 기억이 레이어 입도에서 국소화되어 있다'는 전제를 공유한다. [[extreme-low-bit-quantization]] 계열과 결합하면 양자화가 단순 압축이 아니라 지식 상태의 재해석 변환임이 드러난다. [[model-upgrade-forgetting]]이 의도치 않은 기억 손실을 다룬다면 본 논문은 의도한 제거의 의도치 않은 무효화를 다루어, 지식 지속성의 취약성이 변환 방향에 무관하게 성립하는 동형 구조를 형성한다. 이는 [[learned-safety-revocability]]의 대칭 원리 — 파라미터 상태의 추가와 제거 모두 고정 보장이 아니다 — 를 강화하며, [[configuration-scoped-safety-certification]] 논의에 언러닝 재인증이라는 구체적 사례를 제공한다.

## 🔗 관련 논문

- Don't Drop Dropout: Optimizing Layer Sparsity for Efficient LLMs
- Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study
- Unfolding the Leech Lattice: Fused Multi-Shell Decoding
- Crafting Reversible SFT Behaviors in Large Language Models

## 🏷️ 엔티티

- [[entities/layer-selective-unlearning.md|layer-selective-unlearning]]
- [[entities/adaptive-forgetting.md|adaptive-forgetting]]
- [[entities/selective-forgetting-as-safety.md|selective-forgetting-as-safety]]
- [[entities/model-pruning.md|model-pruning]]
- [[entities/layer-dropout.md|layer-dropout]]
- [[entities/extreme-low-bit-quantization.md|extreme-low-bit-quantization]]
- [[entities/model-upgrade-forgetting.md|model-upgrade-forgetting]]
- [[entities/fact-memorization.md|fact-memorization]]
- [[entities/configuration-scoped-safety-certification.md|configuration-scoped-safety-certification]]
- [[entities/learned-safety-revocability.md|learned-safety-revocability]]

## 📐 개념

- [[concepts/quantization-induced-resurgence.md|quantization-induced-resurgence]]
- [[concepts/parametric-level-forgetting.md|parametric-level-forgetting]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-10-meclear-cooperative-game-theoretic-attribution-and]]: 둘 다 '유틸리티 손실 없이 필요한 것만 잊는' 선택적 망각을 다루며, MeClear가 외부 메모리의 음의 기여 기억 제거라면 본 논문은 파라미터 수준의 레이어 선택적 언러닝으로 망각의 계층을 확장한다.
