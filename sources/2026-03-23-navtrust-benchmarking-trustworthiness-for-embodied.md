# NavTrust: Benchmarking Trustworthiness for Embodied Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19229v1

## 💡 핵심 인사이트

체화된 내비게이션 시스템의 실환경 배포를 위해, 이상적 조건이 아닌 체계적 입력 손상 하에서의 신뢰성 평가가 필수적이며, NavTrust는 VLN과 OGN을 통합하는 최초의 강건성 벤치마크를 제시한다.

## 📖 분석

## NavTrust: Benchmarking Trustworthiness for Embodied Navigation

NavTrust는 체화된 내비게이션(Embodied Navigation) 시스템의 **신뢰성(trustworthiness)**을 체계적으로 평가하기 위한 통합 벤치마크이다. 기존 연구들이 이상적인 조건에서의 성능만 평가해온 것과 달리, NavTrust는 실제 환경에서 발생할 수 있는 다양한 입력 손상(corruption)을 체계적으로 시뮬레이션하여 모델의 강건성을 측정한다.

### 핵심 구조

NavTrust는 두 가지 주요 내비게이션 패러다임을 모두 다룬다:
- **Vision-Language Navigation (VLN)**: 자연어 지시를 따라 이동하는 에이전트
- **Object-Goal Navigation (OGN)**: 지정된 목표 객체를 향해 이동하는 에이전트

벤치마크는 입력 모달리티(시각, 언어, 센서 등)에 대한 체계적 손상을 적용하여, 명목적(nominal) 조건과 손상 조건 간의 성능 격차를 정량화한다. 이는 [[concepts/embodied-ai.md|embodied ai]] 분야에서 실용적 배포를 위한 중요한 평가 프레임워크를 제공한다.

### 기존 연구와의 관계

본 연구는 [[concepts/vision-language-model.md|vision language model]]과 [[concepts/spatial-reasoning.md|spatial reasoning]]의 교차점에 위치하며, AgentVLN이 제시한 에이전틱 VLN 접근법의 강건성을 평가하는 보완적 역할을 한다. 또한 [[concepts/ai-safety.md|ai safety]] 관점에서 내비게이션 모델의 신뢰성 문제를 다루며, TraceSafe가 LLM 가드레일을 평가한 것처럼 체화된 AI 시스템의 안전성 평가 방법론을 확장한다. CADENCE(context-adaptive depth estimation) 연구와도 내비게이션 환경에서의 인식 강건성이라는 주제로 연결된다.

## 🔗 관련 논문

- 2026 04 10 cadence context adaptive depth estimation for navi
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 appear2meaning a cross cultural benchmark for stru

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]
- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/multimodal-learning.md|multimodal-learning]]

---
_LLM 분석으로 재생성됨_
