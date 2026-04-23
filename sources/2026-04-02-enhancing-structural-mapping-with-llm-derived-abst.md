# Enhancing Structural Mapping with LLM-derived Abstractions for Analogical Reasoning in Narratives

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.29997v1

## 💡 핵심 인사이트

LLM의 추상화 능력과 기호적 구조 매핑 엔진의 결합이 서사 간 유추 추론의 표면적 유사성 의존도를 줄이고 깊은 구조적 유추를 가능하게 한다.

## 📖 분석

## Enhancing Structural Mapping with LLM-derived Abstractions for Analogical Reasoning in Narratives

본 논문은 서사(narrative) 간 유추적 추론(analogical reasoning)에서 구조적 매핑(structural mapping)을 LLM 기반 추상화로 강화하는 방법을 제안한다. 유추적 추론은 인간의 일반화 능력의 핵심 메커니즘이지만, 기계에게는 여전히 난제이다. 기존 인지 엔진(cognitive engine)의 구조적 매핑은 사전 추출된 엔티티를 전제로 하며, LLM은 프롬프트 형식과 표면적 유사성(surface similarity)에 민감하다는 한계가 있다.

이 연구는 두 접근법의 간극을 메우기 위해, LLM이 서사에서 추상적 구조 표현을 추출하고 이를 구조적 매핑 엔진에 입력하는 하이브리드 파이프라인을 탐구한다. 핵심 질문은 'LLM이 생성한 추상화가 구조적 매핑의 품질에 어떤 영향을 미치는가'이다.

이는 LLM의 추론 능력과 기호적(symbolic) 인지 모델의 결합이라는 점에서, 최근 [[concepts/reasoning-chain.md|reasoning chain]] 및 [[concepts/reasoning-integrity.md|reasoning integrity]] 연구 흐름과 맥을 같이한다. 특히 Box Maze의 process-control-architecture처럼 LLM 추론의 신뢰성을 외부 구조로 보완하는 전략과 유사한 설계 철학을 공유한다. 또한 [[concepts/theory-of-mind.md|theory of mind]] 연구(Learning Dynamic Belief Graphs)와도 연결되는데, 서사 이해에서 등장인물의 관계와 의도를 구조적으로 파악해야 한다는 점에서 공통 과제를 다룬다.

[[concepts/prompt-engineering.md|prompt engineering]] 관점에서도 의미 있는 기여를 한다. LLM의 유추 성능이 프롬프트 형식에 민감하다는 발견은, 프롬프트 설계가 단순한 지시문 최적화를 넘어 인지적 추상화 수준까지 고려해야 함을 시사한다.

## 🔗 관련 논문

- 2026 03 22 box maze a process control architecture for reliab
- 2026 03 24 learning dynamic belief graphs for theory of mind
- 2026 03 25 evaluating the reliability and fidelity of automat
- 2026 03 25 causal evidence that language models use confidenc

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/analogical-reasoning.md|analogical-reasoning]]
- [[concepts/structural-mapping.md|structural-mapping]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/cognitive-modeling.md|cognitive-modeling]]

---
_LLM 분석으로 재생성됨_
