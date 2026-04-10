# LensWalk: Agentic Video Understanding by Planning How You See in Videos

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24558v1

## 💡 핵심 인사이트

비디오 이해에서 정적 전처리 대신 LLM 추론기가 '어떻게 볼 것인가'를 동적으로 계획하는 에이전틱 지각 패러다임을 제시하여, 추론과 지각의 단절 문제를 해소한다.

## 📖 분석

## LensWalk: Agentic Video Understanding by Planning How You See in Videos

LensWalk는 비디오 이해를 위한 에이전틱 프레임워크로, LLM 추론기가 비디오에서 능동적으로 시각적 증거를 탐색할 수 있도록 설계되었다. 기존 비디오 이해 방식이 정적으로 전처리된 정보에 의존하는 반면, LensWalk는 추론(reasoning)과 지각(perception)의 단절 문제를 해결하기 위해 '어떻게 볼 것인가'를 계획하는 접근법을 도입한다.

### 기존 연구와의 관계

이 연구는 기존 Wiki의 [[video-vlm]], [[vision-language-model]], [[agentic-vlm]] 개념과 직접적으로 연결된다. 특히 VideoSeek가 도구 기반 탐색(tool-guided seeking)으로 장시간 비디오를 처리한 것과 유사하게, LensWalk도 에이전트가 비디오 내 필요한 구간을 능동적으로 선택하는 전략을 취한다. VideoAtlas의 계층적 비디오 탐색과도 맥락을 공유하며, Act Wisely의 메타인지적 도구 사용 개념이 비디오 지각 계획에 적용된 사례로 볼 수 있다.

### 핵심 차별점

기존 video-vlm 연구들이 토큰 압축([[token-pruning]])이나 계층적 표현([[hierarchical-representation]])으로 효율성을 추구한 반면, LensWalk는 에이전트의 추론 과정 자체가 지각 전략을 동적으로 결정하는 '계획 기반 지각(planned perception)' 패러다임을 제시한다. 이는 [[embodied-ai]]의 능동 지각(active perception) 개념을 비디오 이해 영역으로 확장한 것이다.

## 🔗 관련 논문

- VideoSeek: Long-Horizon Video Agent with Tool-Guided Seeking
- VideoAtlas: Navigating Long-Form Video in Logarithmic Comput
- Unified Spatio-Temporal Token Scoring for Efficient Video VL
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- AgentVLN: Towards Agentic Vision-and-Language Navigation

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/video-vlm.md|video-vlm]]
- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/long-context.md|long-context]]
- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/metacognition.md|metacognition]]

---
_LLM 분석으로 재생성됨_
