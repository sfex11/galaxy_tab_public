# SpecEyes: Accelerating Agentic Multimodal LLMs via Speculative Perception and Planning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-26
**링크**: http://arxiv.org/abs/2603.23483v1

## 💡 핵심 인사이트

speculative decoding의 '추측 후 검증' 패러다임을 토큰 수준에서 에이전트 파이프라인 수준으로 확장하여, 멀티모달 에이전트의 인식-추론-도구호출 루프를 병렬화하는 새로운 가속 계층을 제시했다.

## 📖 분석

## SpecEyes: 에이전틱 MLLM을 위한 추측적 가속 프레임워크

SpecEyes는 에이전틱 멀티모달 LLM(예: OpenAI o3, Gemini Agentic Vision)의 반복적 시각 도구 호출에서 발생하는 순차적 오버헤드를 해결하기 위한 프레임워크다. 핵심 개념은 **agentic depth**로, 인식(perception)→추론(reasoning)→도구 호출(tool-calling) 루프가 캐스케이드 방식으로 반복되며 발생하는 지연과 동시성 제한을 정량화한다.

기존 speculative decoding이 토큰 수준에서 병렬화를 달성했다면, SpecEyes는 이를 **에이전트 수준**으로 확장하여 인식과 계획을 동시에 추측적으로 실행한다. 이는 speculative decoding의 개념적 계보를 잇되, 단일 모델의 디코딩이 아닌 멀티모달 에이전트 파이프라인 전체의 가속에 초점을 맞춘다는 점에서 차별화된다.

agentic-vlm 연구 흐름에서 MARCUS가 의료 영역의 에이전틱 VLM 설계를, Act Wisely가 메타인지적 도구 사용 전략을 다루었다면, SpecEyes는 이러한 에이전틱 MLLM 시스템의 **추론 효율성**이라는 시스템 레벨 병목을 직접 공략한다. Nemotron-Cascade 2의 cascade 추론 최적화와도 사상이 맞닿아 있으며, Chimera의 지연 시간-성능 트레이드오프 연구와 상호 참조할 수 있다.

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic Models
- MARCUS: An agentic, multimodal vision-language model for cardiac CT analysis
- Efficient Training-Free Multi-Token Prediction via Embedding
- Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and M
- Chimera: Latency-and Performance-

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/speculative-decoding.md|speculative-decoding]]
- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/multimodal-llm.md|multimodal-llm]]

---
_LLM 분석으로 재생성됨_
