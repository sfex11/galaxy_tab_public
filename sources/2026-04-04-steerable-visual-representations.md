# Steerable Visual Representations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02327v1

## 💡 핵심 인사이트

사전학습 ViT의 범용 시각 표현을 언어 신호로 조향하여, Multimodal LLM의 언어 중심 편향 없이도 특정 시각 개념에 선택적으로 집중할 수 있는 새로운 표현 제어 패러다임을 제시한다.

## 📖 분석

## Steerable Visual Representations

사전학습된 Vision Transformer(ViT)인 DINOv2, MAE 등은 검색, 분류, 세그멘테이션 등 다양한 다운스트림 태스크에 적용 가능한 범용 이미지 특징을 제공하지만, 이미지 내 가장 두드러진 시각적 단서에 집중하는 경향이 있어 덜 눈에 띄는 관심 개념으로 유도할 방법이 없다. 반면 Multimodal LLM은 텍스트 프롬프트로 안내할 수 있으나, 결과 표현이 언어 중심적이어서 시각적 세밀함을 잃는다.

본 논문은 이 간극을 해소하는 **조향 가능한 시각 표현(Steerable Visual Representations)**을 제안한다. 사전학습된 ViT의 범용 시각 특징을 유지하면서도, 텍스트 등 외부 신호를 통해 표현의 초점을 특정 개념으로 유도할 수 있는 메커니즘을 도입한다.

### 기존 Wiki와의 연결

- **Transformer / ViT 계열**: 기존 [[concepts/transformer.md|transformer]] 엔티티와 직접 관련. ViT 기반 사전학습 모델의 표현력 한계를 다루며, transformer 표현의 제어 가능성이라는 새로운 축을 제시한다.
- **Representation Steering**: 기존 [[concepts/representation-steering.md|representation steering]] 개념이 LLM 내부 활성화 벡터 조향에 초점을 맞춘 반면, 본 논문은 **비전 도메인**에서의 표현 조향을 다룬다는 점에서 상호보완적이다. 특히 [[what-drives-representation-steering]] 논문의 메커니즘적 분석과 비교하면, 모달리티 간 조향 기법의 유사성과 차이를 탐구할 수 있다.
- **Multimodal LLM**: [[concepts/multimodal-llm.md|multimodal llm]] 개념과 연결. 텍스트-비전 간 표현 공간의 상호작용을 다루며, 언어 중심 표현의 한계를 시각 중심으로 보완한다.
- **Vision-Language Model**: [[concepts/vision-language-model.md|vision language model]] 계열 연구와 밀접. VLM이 언어 프롬프트로 시각 표현을 안내하는 기존 방식의 대안을 제시한다.
- **Token Pruning**: [[concepts/token-pruning.md|token pruning]] 연구들이 효율성을 위해 토큰을 선별하는 것과 유사하게, 본 연구는 의미적으로 관련된 시각 특징을 선택적으로 강조한다는 점에서 개념적 연결이 있다.

## 🔗 관련 논문

- What Drives Representation Steering? A Mechanistic Case Stud
- Figures as Interfaces: Toward LLM-Native Artifacts for Scien
- Unified Spatio-Temporal Token Scoring for Efficient Video VL
- F2LLM-v2: Inclusive, Performant, and Efficient Embeddings fo

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/multimodal-llm.md|multimodal-llm]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/text-embedding.md|text-embedding]]

---
_LLM 분석으로 재생성됨_
