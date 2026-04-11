# Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-05
**링크**: http://arxiv.org/abs/2604.02315v1

## 💡 핵심 인사이트

LLM 평가의 사각지대를 드러내는 연구로, 어시스턴트 턴만 측정하는 기존 벤치마크를 넘어 유저 턴 생성을 통해 모델의 상호작용 인식(interaction awareness) 여부를 프로빙하는 새로운 평가 패러다임을 제안한다.

## 📖 분석

## Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

기존 LLM 벤치마크는 어시스턴트 턴(모델 응답)만 평가하는 패러다임에 머물러 있다. 본 논문은 이 한계를 지적하며, **유저 턴 생성(user-turn generation)**이라는 새로운 프로빙 방법을 제안한다. 대화 컨텍스트(유저 질의 + 어시스턴트 응답)가 주어졌을 때, 모델에게 유저 역할로 생성하게 함으로써 모델 가중치에 **상호작용 인식(interaction awareness)**이 인코딩되어 있는지를 측정한다.

이 접근은 기존의 [[llm-benchmark]] 평가가 놓치고 있는 대화 흐름의 양방향성을 포착하려는 시도다. 모델이 단순히 응답을 잘 생성하는 것을 넘어, 대화의 다음 단계—즉 사용자가 어떤 후속 질문이나 반응을 할지—에 대한 내재적 모델링 능력을 갖추고 있는지를 검증한다.

[[metacognition]] 연구(Act Wisely 등)가 모델의 자기 인식 능력을 탐구했다면, 본 연구는 **타자 인식(other-awareness)**으로 확장한다. [[reasoning-chain-evaluation]] 관점에서도, 어시스턴트 응답의 품질이 후속 유저 턴 예측 정확도와 상관관계를 보이는지가 핵심 질문이 된다. 또한 [[theory-of-mind]] 연구와도 연결되는데, 유저 턴 생성은 본질적으로 대화 상대방의 의도와 기대를 모델링하는 능력을 테스트하기 때문이다.

기존 [[llm-alignment]] 연구가 모델 출력의 유용성·안전성에 집중했다면, 본 논문은 평가 방법론 자체의 사각지대를 조명한다는 점에서 보완적이다.

## 🔗 관련 논문

- What do Language Models Learn and When? The Implicit Curricu
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Evaluating the Reliability and Fidelity of Automated Judgmen
- What Drives Representation Steering? A Mechanistic Case Stud
- Box Maze: A Process-Control Architecture for Reliable LLM Re

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/reasoning-chain-evaluation.md|reasoning-chain-evaluation]]
- [[concepts/theory-of-mind.md|theory-of-mind]]
- [[concepts/llm-alignment.md|llm-alignment]]

---
_LLM 분석으로 재생성됨_
