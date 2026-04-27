# From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-27
**링크**: http://arxiv.org/abs/2604.21910v1

## 💡 핵심 인사이트

과학 자동화의 실질적 병목은 실행 엔지니어링이 아니라 연구 질문을 형식적 명세로 번역하는 의미론적 변환 과정이며, 이를 LLM을 외부 번역 계층으로, validated generator를 내부 무결성 계층으로 분리하는 3층 아키텍처로 해결한다.

## 📖 분석

## From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation (2026-04-27)

본 논문은 과학 워크플로우 자동화의 핵심 병목을 '실행 자동화'가 아닌 '의미론적 번역 자동화'로 규정한다는 점에서 기존 분석의 핵심을 확인시킨다. 기존 Wiki에서 이미 3층 아키텍처(의미→명세→실행)와 autoresearch 스코프 확장을 포착했으나, 본 버전에서는 두 가지 교차 연결이 가능하다.

첫째, [[entities/external-layer-principle|외부 계층 원칙]]의 구체적 실현 사례다. LLM이 워크플로우를 직접 실행하지 않고 '구조화된 의도' 생성에만 국한하는 설계는, LLM을 형식 체계의 외부 계층에 위치시킨다는 아키텍처 원칙을 과학 자동화 도메인에서 실증한다. 둘째, [[concepts/semantic-translation-gap|의미론적 번역 간극]]을 [[concepts/epistemic-gap|인식론적 단절]]과 구조적으로 연결할 수 있다 — 둘 다 '표현과 현실 사이의 구조적 불일치'를 기술하지만, 전자는 명세 생성 시점에서, 후자는 인지 모델 검증 시점에서 발생한다.

또한 'validated generators'라는 표현은 [[entities/formal-verification|형식적 검증]]과 [[concepts/reproducible-specification-generation|재현 가능 명세 생성]]의 교차점을 시사하며, 단순한 자연어 변환을 넘어 명세의 형식적 무결성을 보장하는 계층이 존재함을 암시한다.

## 🔗 관련 논문

- 2026 04 25 from research question to scientific workflow leve
- 2026 04 26 from research question to scientific workflow leve
- 2026 04 24 automatic ontology construction using llms as an e
- 2026 04 25 bounding the black box a statistical certification
- 2026 04 10 syntax is easy semantics is hard evaluating llms f

## 🏷️ 엔티티

- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/external-layer-principle.md|external-layer-principle]]
- [[entities/formal-verification.md|formal-verification]]

## 📐 개념

- [[concepts/semantic-translation-gap.md|semantic-translation-gap]]
- [[concepts/three-layer-agentic-workflow.md|three-layer-agentic-workflow]]
- [[concepts/intent-structured-specification.md|intent-structured-specification]]
- [[concepts/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[concepts/epistemic-gap.md|epistemic-gap]]

---
_LLM 분석으로 생성됨_
