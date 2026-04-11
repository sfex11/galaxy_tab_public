# Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02315v1

## 💡 핵심 인사이트

LLM 평가를 어시스턴트 턴에서 유저 턴 생성으로 확장하면, 모델이 대화의 양방향 역학을 얼마나 인코딩하고 있는지(interaction awareness)를 측정할 수 있는 새로운 평가 축이 열린다.

## 📖 분석

## Beyond the Assistant Turn: User Turn Generation as a Probe of Interaction Awareness in Language Models

기존 LLM 벤치마크는 어시스턴트 턴(assistant turn)만 평가한다: 모델이 입력에 대한 응답을 생성하고, 검증기가 정확성을 채점하면 분석이 끝난다. 본 논문은 이 패러다임이 **어시스턴트 응답 이후에 무엇이 올지에 대한 모델의 인식**을 측정하지 못한다는 점을 지적한다. 이를 해결하기 위해 **유저 턴 생성(user-turn generation)**이라는 프로브를 제안한다: 사용자 질의와 어시스턴트 응답으로 구성된 대화 컨텍스트가 주어지면, 모델이 사용자 역할로 생성하도록 한다. 모델의 가중치가 상호작용 인식(interaction awareness)을 인코딩하고 있다면, 생성된 유저 턴이 대화의 자연스러운 흐름을 반영할 것이다.

이 연구는 LLM 평가 방법론에 근본적인 질문을 던진다. 기존 [[llm-benchmark]] 관련 연구들이 모델의 출력 품질만 측정했다면, 본 논문은 모델이 **대화의 양방향 역학**을 얼마나 이해하는지를 탐구한다. 이는 [[reasoning-integrity]]와도 연결되는데, 모델이 단순히 정답을 생성하는 것을 넘어 대화 맥락 전체를 파악하는 능력을 검증하기 때문이다. 또한 [[llm-agent]] 연구에서 에이전트가 사용자 의도를 예측하고 선제적으로 대응해야 하는 상황과 직결된다. [[metacognition]] 연구와도 접점이 있어, 모델이 자신의 응답이 후속 상호작용에 미치는 영향을 인식하는지를 평가하는 새로운 축을 제공한다.

## 🔗 관련 논문

- 2026 04 10 chatbot based assessment of code understanding in
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 11 what do language models learn and when the implici
- 2026 03 22 box maze a process control architecture for reliab

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/interaction-awareness.md|interaction-awareness]]

---
_LLM 분석으로 재생성됨_
