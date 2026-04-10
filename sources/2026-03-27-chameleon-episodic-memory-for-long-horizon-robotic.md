# Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24576v1

## 💡 핵심 인사이트

로봇 조작에서 의미 압축 기반 메모리 대신 원시 지각 단서를 보존하는 에피소딕 메모리가 관찰 수준의 비마르코프 의사결정 문제를 효과적으로 해결한다.

## 📖 분석

## Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation

로봇 조작(manipulation) 태스크에서 **에피소딕 메모리(episodic memory)**를 활용하여 장기 시계(long-horizon) 문제를 해결하는 프레임워크를 제안한다. 기존 embodied agent들은 의미적으로 압축된 트레이스(semantically compressed traces)와 유사도 기반 검색(similarity-based retrieval)을 메모리로 사용하지만, 이는 결정에 필요한 세밀한 지각 단서(fine-grained perceptual cues)를 버리고 지각적으로 유사하지만 의사결정과 무관한 에피소드를 반환하는 문제가 있다.

Chameleon은 이 문제를 **관찰 수준의 비마르코프성(non-Markovian at observation level)**으로 정의한다. 동일한 관찰이 서로 다른 상호작용 이력에서 발생할 수 있어 행동 선택이 현재 관찰만으로는 불가능한 상황을 다룬다. 이를 해결하기 위해 에피소딕 메모리를 도입하여 과거 상호작용의 원시 지각 정보를 보존하고, 현재 의사결정 맥락에 맞는 관련 에피소드를 검색한다.

이 연구는 기존의 ChameleonEpisodicMemoryforLong 관련 연구들과 달리, 의미 압축 대신 **원시 지각 단서 보존**을 강조하며, 폐색(occlusion)과 상태 변화로 인한 지각적 앨리어싱(perceptual aliasing) 문제에 초점을 맞춘다. 이는 VLM 기반 에이전트의 메모리 설계에서 '무엇을 기억할 것인가'와 '어떻게 검색할 것인가'의 트레이드오프를 재고하게 한다. 로봇 조작의 장기 시계 태스크에서 메모리 아키텍처가 성능에 미치는 영향을 실증적으로 보여준다.

## 🔗 관련 논문

- AgentVLN: Towards Agentic Vision-and-Language Navigation
- PSI: Shared State as the Missing Layer for Coherent AI-Gener
- Visually-grounded Humanoid Agents
- ChameleonEpisodicMemoryforLong-slides.html

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]
- [[entities/vlm.md|vlm]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/long-context.md|long-context]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
