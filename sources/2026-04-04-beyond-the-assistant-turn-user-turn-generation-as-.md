# Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02315v1

## 💡 핵심 인사이트

LLM 평가의 패러다임을 어시스턴트 턴에서 유저 턴 생성으로 확장함으로써, 모델이 대화 상호작용의 후속 흐름을 인식하는 능력(interaction awareness)을 측정할 수 있는 새로운 프로빙 방법론을 제시했다.

## 📖 분석

## Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

기존 LLM 벤치마크는 **어시스턴트 턴**(모델의 응답)만 평가하는 패러다임에 머물러 있다. 본 논문은 이 한계를 지적하며, **유저 턴 생성(user-turn generation)**이라는 새로운 프로빙 방법을 제안한다. 대화 컨텍스트(유저 질의 + 어시스턴트 응답)가 주어졌을 때 모델이 유저 역할로 생성하도록 하여, 모델 가중치에 **상호작용 인식(interaction awareness)**이 인코딩되어 있는지를 측정한다.

이는 기존 [[concepts/llm-benchmark.md|llm benchmark]] 연구가 단방향 평가에 치우쳐 있다는 근본적 문제를 제기한다. 모델이 단순히 정답을 생성하는 능력뿐 아니라, 대화의 후속 흐름을 예측하고 이해하는 능력까지 평가해야 한다는 주장이다. [[concepts/metacognition.md|metacognition]] 연구와 연결되는데, 모델이 자신의 응답이 유저에게 어떤 후속 반응을 유발할지 인식하는 것은 일종의 메타인지적 능력에 해당한다.

[[concepts/reasoning-chain-evaluation.md|reasoning chain evaluation]] 관점에서도 의미가 크다. 기존에는 추론 체인의 최종 출력만 평가했다면, 유저 턴 생성은 대화적 맥락에서의 추론 연속성을 평가하는 새로운 축을 제공한다. 또한 [[concepts/theory-of-mind.md|theory of mind]] 연구와도 밀접하게 연관되는데, 유저의 다음 발화를 예측하려면 유저의 의도와 만족도를 모델링해야 하기 때문이다.

이 연구는 LLM 평가 방법론의 사각지대를 조명하며, 챗봇 품질 평가와 RLHF 보상 모델 설계에도 실질적 시사점을 제공한다.

## 🔗 관련 논문

- Evaluating the Reliability and Fidelity of Automated Judgmen
- Box Maze: A Process-Control Architecture for Reliable LLM Re
- Causal Evidence that Language Models use Confidence to Drive
- Learning Dynamic Belief Graphs for Theory-of-mind Reasoning
- What do Language Models Learn and When? The Implicit Curricu
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/reasoning-chain-evaluation.md|reasoning-chain-evaluation]]
- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/interaction-awareness.md|interaction-awareness]]
- [[concepts/user-turn-generation.md|user-turn-generation]]

---
_LLM 분석으로 재생성됨_
