# VISion On Request: Enhanced VLLM efficiency with sparse, dynamically selected, vision-language interactions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23495v1

## 💡 핵심 인사이트

시각 토큰을 제거하는 대신 레이어별 시각-언어 상호작용을 동적으로 선택함으로써, 정보 손실 없이 LVLM 추론 효율을 개선할 수 있다는 새로운 패러다임을 제시한다.

## 📖 분석

## VISion On Request (VISOR): 시각 토큰 축소 없는 LVLM 효율화

VISOR는 기존 Large Vision-Language Model(LVLM) 효율화의 지배적 패러다임인 **시각 토큰 축소(visual token reduction)**에 정면으로 도전하는 연구다. 기존 접근법들이 시각 토큰을 압축·제거하여 연산 비용을 줄이는 반면, VISOR는 시각 정보를 버리지 않으면서도 추론 비용을 절감한다. 핵심 아이디어는 모든 레이어에서 시각-언어 상호작용(cross-attention)을 수행하는 대신, **필요한 레이어에서만 선택적으로(sparse, dynamically)** 시각 정보를 참조하는 것이다.

이는 기존 token-pruning 계열 연구([[concepts/token-pruning.md|token pruning]])가 직면하는 정보 병목(information bottleneck) 문제를 근본적으로 우회한다. 특히 세밀한 이해와 추론이 필요한 어려운 태스크에서 토큰 축소 방식의 성능 저하가 심한데, VISOR는 전체 시각 정보를 유지하므로 이 한계를 극복한다.

기존 Wiki의 [[concepts/vision-language-model.md|vision language model]], [[entities/vlm.md|vlm]], [[entities/mllm.md|mllm]] 엔티티와 직접 관련되며, Unified Spatio-Temporal Token Scoring 등 video-vlm 효율화 연구와도 비교 가능하다. 다만 VISOR는 토큰 자체를 줄이는 것이 아니라 **어텐션 연산의 희소화**라는 직교적 전략을 취한다는 점에서 차별화된다. Transformer 아키텍처 내 cross-attention 메커니즘의 동적 제어라는 측면에서 [[concepts/transformer.md|transformer]] 엔티티와도 연결된다.

## 🔗 관련 논문

- 2026 03 19 unified spatio temporal token scoring for efficien
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 09 mmemb r1 reasoning enhanced multimodal embedding w

## 🏷️ 엔티티

- [[entities/vlm.md|VLM]]
- [[entities/mllm.md|MLLM]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/video-vlm.md|video-vlm]]

---
_LLM 분석으로 재생성됨_
