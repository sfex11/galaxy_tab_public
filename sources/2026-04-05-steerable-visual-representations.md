# Steerable Visual Representations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-05
**링크**: http://arxiv.org/abs/2604.02327v1

## 💡 핵심 인사이트

ViT의 범용 시각 특징을 텍스트 조건부 경량 어댑터로 조종함으로써, MLLM의 언어 중심성과 순수 ViT의 비유도성 사이의 간극을 메우는 새로운 표현 패러다임을 제시한다.

## 📖 분석

## Steerable Visual Representations

사전학습된 Vision Transformer(ViT)인 DINOv2, MAE 등은 범용 이미지 특징을 제공하지만, 이미지 내 가장 두드러진 시각적 단서에 집중하는 경향이 있어 특정 개념으로 유도하기 어렵다. 반면 Multimodal LLM은 텍스트 프롬프트로 안내할 수 있지만 언어 중심적 표현이 되어 시각적 세밀함을 잃는다. 본 논문은 이 간극을 메우는 **조종 가능한 시각 표현(Steerable Visual Representations)**을 제안한다.

핵심 아이디어는 경량 어댑터를 통해 ViT의 범용 시각 특징을 텍스트 조건부로 특정 개념 방향으로 유도하는 것이다. 이는 기존 [[concepts/representation-steering|representation-steering]] 연구가 주로 LLM 내부 활성화 조종에 집중한 것과 달리, **비전 인코더 출력 공간**에서의 조종이라는 점에서 차별화된다. [[entities/transformer|Transformer]] 아키텍처 기반 ViT를 활용하되, [[entities/mllm|MLLM]]과 달리 시각적 충실도를 유지하면서도 언어적 유도가 가능한 중간 지점을 제시한다.

검색, 분류, 세그멘테이션 등 다양한 다운스트림 태스크에 적용 가능하며, [[concepts/multimodal-learning|multimodal-learning]]과 [[concepts/text-embedding|text-embedding]] 분야를 연결하는 실용적 접근법이다. 특히 [[concepts/vision-language-model|vision-language-model]] 패러다임에서 시각 표현의 조종 가능성이라는 새로운 축을 추가한다.

## 🔗 관련 논문

- What Drives Representation Steering? A Mechanistic Case Study
- Aligned, Orthogonal or In-conflict: When can we safely steer
- Analysing the Safety Pitfalls of Steering Vectors
- Unified Spatio-Temporal Token Scoring for Efficient Video VL
- Feeling the Space: Egomotion-Aware Video Representation for
- F2LLM-v2: Inclusive, Performant, and Efficient Embeddings fo

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]
- [[entities/vlm.md|vlm]]
- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/text-embedding.md|text-embedding]]
- [[concepts/token-pruning.md|token-pruning]]

---
_LLM 분석으로 재생성됨_
