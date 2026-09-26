# Agentic Detection of Online Conspiracies

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30250v1

## 💡 핵심 인사이트

음모론 담화 탐지의 본질적 과제는 콘텐츠 인식이 아니라 화행력(화자 의도) 추론이며, 동일한 표면 텍스트가 지지·우려·풍자·조롱으로 다의적이므로 사회적 맥락에 근거한 에이전틱 의도 추론이 필요하다.

## 📖 분석

온라인 음모론 탐지를 위한 에이전틱 프레임워크를 제시한다. 핵심 진단: 소셜 미디어의 음모론 담화는 명시적 주장이나 안정적 어휘 마커로 표현되지 않으며, 동일한 표면 콘텐츠가 지지(endorsement), 정당한 우려, 비판, 풍자, 조롱 등 서로 다른 화행력(illocutionary force)을 운반할 수 있다. 따라서 과제의 본체는 음모론 주장 인식이 아니라 화자 의도 추론이며, 해법으로 사회적 맥락을 활용하는 에이전틱 프레임워크를 제안한다.

이는 Wiki의 구조 원리들과 정합적이다. [[single-surface-signal-insufficiency]]가 테스트 통과·캡션·CoT 등 단일 표면 신호의 불충분성을 주장했다면, 본 논문은 그 원리가 담화 분석에서 '어휘 마커 → 화자 의도' 간극으로 발현됨을 보여준다. [[intent-execution-coupling-assumption]]이 의도-관측 결합 가정을 비판했다면, 본 논문은 담화 도메인에서 같은 구조(표면-의도 결합 붕괴)를 확인한다: 표면 텍스트는 의도를 결정하지 않는다.

동시에 [[theory-of-mind]]의 담화 확장이다 — 사회적 맥락에 근거한 화자 신념 상태 모델링이 의도 추론의 메커니즘이 된다. [[same-request-same-reading-assumption]]에 대한 담화 버전 반증이기도 하다: 동일 콘텐츠라도 맥락에 따라 판독(지지/풍자/조롱)이 달라지며, 맥락 결합이 판독 타당성의 조건이다.

## 🏷️ 엔티티

- [[entities/illocutionary-force-inference.md|illocutionary-force-inference]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/intent-execution-coupling-assumption.md|intent-execution-coupling-assumption]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/surface-completeness-misreading.md|surface-completeness-misreading]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/illocutionary-force-inference.md|illocutionary-force-inference]]
- [[concepts/surface-intent-decoupling.md|surface-intent-decoupling]]

---
_LLM 분석으로 생성됨_
