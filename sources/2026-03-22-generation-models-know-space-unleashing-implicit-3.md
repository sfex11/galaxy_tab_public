# Generation Models Know Space: Unleashing Implicit 3D Priors for Scene Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19235v1

## 💡 핵심 인사이트

비디오 생성 모델이 학습 과정에서 자연스럽게 획득한 암묵적 3D 공간 프라이어를 명시적 3D 데이터 없이 장면 이해에 전이할 수 있다는 패러다임 전환을 제시한다.

## 📖 분석

## Generation Models Know Space: Unleashing Implicit 3D Priors for Scene Understanding

본 논문은 대규모 비디오 생성 모델 내부에 암묵적으로 내재된 3D 공간 프라이어(implicit 3D prior)를 활용하여 장면 이해(scene understanding) 성능을 향상시키는 새로운 패러다임을 제안한다.

### 핵심 문제
Multimodal Large Language Model(MLLM)은 뛰어난 의미론적 능력을 보이지만, 세밀한 기하학적 추론(geometric reasoning)과 물리적 동역학(physical dynamics) 이해에서 '공간적 맹점(spatial blindness)'을 겪는다. 기존 해결책은 명시적 3D 모달리티나 복잡한 기하학적 스캐폴딩에 의존하나, 데이터 부족과 일반화 한계가 있다.

### 제안 방법
저자들은 명시적 3D 데이터 대신, 대규모 비디오 생성 모델이 학습 과정에서 자연스럽게 획득한 암묵적 공간 프라이어를 활용하는 패러다임 전환을 제안한다. 비디오 생성 모델은 시간적 일관성을 유지하기 위해 3D 구조, 깊이, 카메라 움직임 등에 대한 내재적 이해를 갖추고 있으며, 이를 장면 이해 태스크에 전이(transfer)할 수 있다는 가설에 기반한다.

### 의의
이 접근법은 명시적 3D 감독 신호 없이도 공간 이해 능력을 확보할 수 있어, 데이터 효율성과 일반화 측면에서 이점을 가진다. 생성 모델과 이해 모델의 경계를 허무는 연구 방향으로, diffusion 기반 world model 연구 흐름과 맥을 같이 한다.

## 🔗 관련 논문

- Feeling the Space: Egomotion-Aware Video Representation for 
- Loc3R-VLM: Language-based Localization and 3D Reasoning with
- VectorWorld: Efficient Streaming World Model via Diffusion F
- LoST: Level of Semantics Tokenization for 3D Shapes
- Universal Skeleton Understanding via Differentiable Renderin

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]
- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/3d-scene-understanding.md|3d-scene-understanding]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/diffusion-model.md|diffusion-model]]
- [[concepts/world-model.md|world-model]]
- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/3d-spatial-reasoning.md|3d-spatial-reasoning]]

---
_LLM 분석으로 재생성됨_
