# MARCUS: An agentic, multimodal vision-language model for cardiac diagnosis and management

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22179v1

## 💡 핵심 인사이트

MARCUS는 에이전틱 VLM 패러다임을 임상 심장학에 적용하여, 이질적 의료 모달리티(ECG/초음파/MRI)를 통합 추론하는 대화형 진단 시스템을 구현함으로써 도메인 특화 멀티모달 에이전트의 실현 가능성을 입증했다.

## 📖 분석

## MARCUS: 심장 진단을 위한 에이전틱 멀티모달 비전-언어 모델

MARCUS(Multimodal Autonomous Reasoning and Chat for Ultrasound and Signals)는 심전도(ECG), 심초음파, 심장 MRI를 독립적으로 해석할 수 있는 에이전틱 비전-언어 시스템이다. 기존 의료 AI가 단일 모달리티에 국한되고 비대화형이었던 한계를 극복하여, 다중 심장 검사 데이터를 통합적으로 추론하고 대화형 인터페이스를 제공한다.

### 기존 Wiki와의 관계

본 논문은 [[concepts/vision-language-model.md|vision language model]]과 [[entities/llm-agent.md|llm agent]]의 교차점에 위치한다. 기존 Wiki의 VLM 연구들이 주로 일반 시각-언어 태스크(네비게이션, 3D 추론, 그라운딩)에 집중한 반면, MARCUS는 임상 의료 도메인에 VLM+에이전트 패러다임을 적용한 사례다. [[concepts/multimodal-learning.md|multimodal learning]] 개념과도 밀접하나, 여기서의 멀티모달은 이미지-텍스트가 아닌 ECG 신호, 초음파 영상, MRI 등 이질적 의료 데이터 간 융합이라는 점에서 차별화된다.

에이전틱(agentic) 설계는 [[entities/llm-agent.md|llm agent]] 엔티티 및 [[concepts/tool-use.md|tool use]] 개념과 직접 연결된다. 단순 추론을 넘어 자율적으로 진단 워크플로우를 수행하는 구조는 AgentVLN, AgentFactory 등 기존 에이전트 연구의 의료 도메인 확장으로 볼 수 있다.

### 시사점

의료 AI에서 '단일 모달리티 + 비대화형'이라는 기존 패러다임의 한계를 에이전틱 VLM으로 돌파하려는 시도로, 도메인 특화 멀티모달 에이전트의 가능성을 보여준다.

## 🔗 관련 논문

- 2026 04 09 maestro adapting guis and guiding navigation with
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/medical-ai.md|medical-ai]]
- [[concepts/agentic-vlm.md|agentic-vlm]]

---
_LLM 분석으로 재생성됨_
