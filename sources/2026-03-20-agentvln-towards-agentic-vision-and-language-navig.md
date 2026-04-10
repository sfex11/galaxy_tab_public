# AgentVLN: Towards Agentic Vision-and-Language Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.17670v1

## 💡 핵심 인사이트

VLM 기반 에이전트를 2D 의미 이해에서 3D 공간 내비게이션으로 확장하면서, 에지 컴퓨팅 배포가 가능한 효율적 embodied navigation 프레임워크를 제시한다.

## 📖 분석

## AgentVLN: Towards Agentic Vision-and-Language Navigation

**분류**: Embodied AI, Vision-and-Language Navigation

### 핵심 내용

AgentVLN은 자연어 명령을 기반으로 미지의 환경에서 장기 내비게이션을 수행하는 에이전트 프레임워크다. 기존 VLN 시스템이 갖고 있던 **제한된 공간 인식**, **2D-3D 표현 불일치**, **단안 스케일 모호성** 문제를 해결하기 위해 설계되었다.

### 기술적 접근

Vision-Language Model(VLM)의 강력한 2D 의미 이해 능력을 활용하면서도, 3D 공간 추론과의 간극을 메우는 것이 핵심 과제다. 에지 컴퓨팅 환경에서도 배포 가능한 효율적 구조를 지향하며, embodied agent가 복잡한 자연어 지시를 실제 내비게이션 행동으로 grounding하는 과정을 개선한다.

### 기존 연구와의 관계

LLM Agent 연구의 embodied AI 확장으로 볼 수 있다. 특히 [[entities/llm-agent]]의 물리 환경 적용 사례이며, 언어-비전 정합(grounding) 측면에서 [[sources/2026-04-08-filegram-grounding-agent-personalization-in-file-s|FileGram]]의 grounding 개념과 맥을 같이한다. 또한 에이전트 내비게이션이라는 점에서 [[sources/2026-04-10-cadence-context-adaptive-depth-estimation-for-navi|CADENCE]]의 depth estimation 기술과 상호보완적이다. GUI 에이전트 내비게이션 연구인 [[sources/2026-04-09-maestro-adapting-guis-and-guiding-navigation-with|MAESTRO]]와도 '내비게이션 에이전트'라는 공통 주제를 공유하지만, AgentVLN은 물리 공간에서의 3D 내비게이션에 초점을 맞춘다는 차별점이 있다.

### 의의

VLM 기반 에이전트가 디지털 환경(코드, 웹, GUI)을 넘어 물리 공간으로 확장되는 흐름을 보여주며, 에지 디바이스 배포를 고려한 효율성 설계가 실용적 가치를 높인다.

## 🔗 관련 논문

- 2026 04 08 filegram grounding agent personalization in file s
- 2026 04 10 cadence context adaptive depth estimation for navi
- 2026 04 09 maestro adapting guis and guiding navigation with

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/vision-language-model.md|vision-language-model]]

---
_LLM 분석으로 재생성됨_
