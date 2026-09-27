# Agentic Detection of Online Conspiracies

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30250v1

## 💡 핵심 인사이트

음모론 탐지의 핵심은 표면 콘텐츠가 아니라 음성행위력(화자 의도)의 추론이며, 동일 표면의 다의성은 측정 결함이 아니라 담화의 구조이므로 사회적 맥락을 능동 수집하는 에이전틱 프레임워크가 요구된다.

## 📖 분석

# Agentic Detection of Online Conspiracies (2026-09-27)

온라인 음모론 담화는 명시적 주장이나 안정적 어휘 마커로 표현되지 않는다. 동일한 표면 콘텐츠가 지지, 정당한 우려, 비판, 풍자, 조롱이라는 상이한 음성행위력(illocutionary force)을 가질 수 있다. 따라서 탐지의 핵심 과제는 음모론 주장의 인식이 아니라 **화자 의도의 추론**이며, 본 논문은 이를 관련 사회적 맥락을 능동 수집하는 에이전틱 프레임워크로 해결한다.

## 기존 Wiki와의 관계

[[concepts/illocutionary-force-inference.md|illocutionary force inference]] 엔티티의 원천 논문으로, Wiki 전반의 표면-의도 논의와 공명한다:

- [[concepts/surface-intent-decoupling.md|surface intent decoupling]]: 동일 표면이 5가지 의도로 실현 가능함을 실증 — 표면-의도 탈동조화가 담화의 기본 상태임을 확립
- [[concepts/single-surface-signal-insufficiency.md|single surface signal insufficiency]]: 어휘 마커라는 단일 표면 신호의 불충분성을 콘텐츠 조정 도메인에서 재확인
- [[concepts/same-request-same-reading-assumption.md|same request same reading assumption]]: '같은 요청-같은 판독' 전제의 담화 버전 반증 제공

## 새로운 통찰

판독 변이의 원인을 '계측기의 결함'이 아니라 '담화의 구조'로 재귀인한다. 사회적 맥락에 따라 상이한 판독이 모두 유효하므로, 판독의 비일관성은 다의적 발화의 올바른 반영일 수 있다. 의도 판독은 문자적 내용 판독이 아니라 화자의 의사소통 의도 모델링, 즉 제3자 위치에서의 마음 이론 과제([[concepts/theory-of-mind.md|theory of mind]])이며, 이는 LLM judge의 판독 문제([[concepts/judge-instrument-reliability.md|judge instrument reliability]])가 내용 도메인에서도 성립함을 시사한다.

## 🔗 관련 논문

- Measuring the Serving Stack Instead of the Model: Hidden Con
- Legibility is Not Interpretability: Comparing Judged and Act
- Mind2Dialogue: Training Human-Aware Language Models by Simul

## 🏷️ 엔티티

- [[entities/illocutionary-force-inference.md|illocutionary-force-inference]]
- [[entities/surface-intent-decoupling.md|surface-intent-decoupling]]
- [[entities/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/surface-completeness-misreading.md|surface-completeness-misreading]]
- [[entities/intent-execution-coupling-assumption.md|intent-execution-coupling-assumption]]
- [[entities/theory-of-mind.md|theory-of-mind]]

## 📐 개념

- [[concepts/illocutionary-force-inference.md|illocutionary-force-inference]]
- [[concepts/surface-intent-decoupling.md|surface-intent-decoupling]]
- [[concepts/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/surface-completeness-misreading.md|surface-completeness-misreading]]
- [[concepts/intent-execution-coupling-assumption.md|intent-execution-coupling-assumption]]
- [[concepts/theory-of-mind.md|theory-of-mind]]

---
_LLM 분석으로 생성됨_
