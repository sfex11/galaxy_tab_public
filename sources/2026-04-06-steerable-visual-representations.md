# Steerable Visual Representations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02327v1

## 💡 핵심 인사이트

ViT의 범용 시각 특징과 멀티모달 LLM의 텍스트 유도 능력을 결합하여, 언어 조건부로 특정 시각 개념에 주의를 조종할 수 있는 표현 학습 프레임워크를 제시한다.

## 📖 분석

## Steerable Visual Representations

사전학습된 Vision Transformer(ViT)인 DINOv2, MAE 등은 검색, 분류, 세그멘테이션 등 다양한 다운스트림 태스크에 활용 가능한 범용 이미지 특징을 제공한다. 그러나 이러한 표현은 이미지 내 가장 두드러진 시각적 단서에 집중하는 경향이 있어, 덜 두드러진 관심 개념으로 유도할 방법이 없다. 반면 멀티모달 LLM은 텍스트 프롬프트로 가이드할 수 있지만, 결과 표현이 언어 중심적이어서 순수 시각적 정보가 손실되는 한계가 있다.

본 연구는 이 두 패러다임의 간극을 메우는 **조종 가능한 시각 표현(Steerable Visual Representations)**을 제안한다. 핵심 아이디어는 ViT의 범용 시각 특징을 유지하면서도, 텍스트 조건부로 특정 시각 개념에 주의를 기울이도록 표현을 조종(steer)하는 것이다. 이는 representation steering 개념을 시각 도메인으로 확장한 것으로, LLM에서의 활성화 조종 연구([[What Drives Representation Steering]])와 맥을 같이한다.

이 접근은 기존 Transformer 기반 비전 모델의 표현력을 재활용하면서 멀티모달 LLM의 유연성을 결합한다는 점에서, token pruning 기반 효율화 연구나 VLM 연구와도 접점을 가진다. 특히 에이전틱 VLM([[Act Wisely]])이 도구 선택 시 시각 표현의 질에 의존하는 만큼, 조종 가능한 표현은 에이전트의 상황 인식 정확도를 높이는 기반 기술이 될 수 있다.

## 🔗 관련 논문

- What Drives Representation Steering? A Mechanistic Case Stud
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Unified Spatio-Temporal Token Scoring for Efficient Video VL
- Aligned, Orthogonal or In-conflict: When can we sa
- Analysing the Safety Pitfalls of Steering Vectors

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/representation-steering.md|representation-steering]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/multimodal-llm.md|multimodal-llm]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/agentic-vlm.md|agentic-vlm]]

---
_LLM 분석으로 재생성됨_
