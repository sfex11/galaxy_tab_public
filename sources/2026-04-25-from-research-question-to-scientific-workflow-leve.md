# From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21910v1

## 💡 핵심 인사이트

과학 자동화의 병목은 워크플로우 실행이 아니라 연구 질문을 워크플로우 사양으로 변환하는 의미론적 번역에 있으며, 이를 LLM 기반 3층 에이전트 아키텍처로 해결하여 autoresearch를 발견→명세화→실행의 완전한 파이프라인으로 확장한다.

## 📖 분석

# From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation

## 핵심 기여

기존 과학 워크플로우 시스템은 실행 자동화(스케줄링, 장애 복구, 리소스 관리)만 수행하고, 연구 질문을 워크플로우 사양으로 변환하는 **의미론적 번역(semantic translation)**은 여전히 수동에 의존한다는 간극을 식별한다. 이 간극을 3층 에이전트 아키텍처로 해결한다: (1) LLM이 자연어를 구조적 의도로 해석하는 의미 계층, (2) 검증된 생성기가 재현 가능한 워크플로우 사양을 산출하는 생성 계층, (3) 실행 계층.

## 기존 Wiki와의 관계

### autoresearch와의 보완성
기존 [[entities/llm-agent|LLM Agent]] 생태계의 autoresearch 논문들(Bilevel Autoresearch, Claudini)은 연구 발견(논문 탐색, 가설 생성)에 집중했다. 본 논문은 그 다음 단계—발견된 연구 질문을 실행 가능한 워크플로우로 변환하는 명세화(specification) 단계—를 자동화하여, autoresearch가 **발견→명세화→실행**의 3단계로 분해되어야 함을 시사한다.

### workflow-engineering-automation의 구체화
기존 [[concepts/workflow-engineering-automation|workflow-engineering-automation]] 개념을 과학 도메인에 특화하여 구체화한다. 비즈니스 요구사항→파이프라인이 아닌, 연구 질문→과학 워크플로우라는 변환의 '소스 언어'가 가진 고유한 난점(도메인 지식과 인프라 전문성의 병행 요구)을 명시적으로 다룬다.

### natural-language-to-formal-language의 확장
기존 [[concepts/natural-language-to-formal-language|natural-language-to-formal-language]] 변환(예: LTL 번역)이 형식 언어의 구문론적 정확성에 집중한 반면, 본 논문은 **재현성(reproducibility)**을 핵심 제약으로 추가한다. 과학 워크플로우에서 구문론적 정확성만으로는 부족하고, 생성된 사양이 동일 결과를 재현할 수 있어야 한다는 도메인 특화적 요구사항을 제시한다.

### QRafti와의 연결
Wiki 소스 목록의 "qrafti an agentic framework for empirical research"와 직접적으로 연결된다. QRafti가 경험적 연구의 전체 파이프라인을 다룬다면, 본 논문은 그 파이프라인 내에서 연구 질문→워크플로우 명세 변환에 대한 이론적 프레이밍을 제공한다.

## 🔗 관련 논문

- 2026 04 22 qrafti an agentic framework for empirical research

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]

## 📐 개념

- [[concepts/semantic-workflow-translation.md|semantic-workflow-translation]]
- [[concepts/workflow-engineering-automation.md|workflow-engineering-automation]]
- [[concepts/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[concepts/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[concepts/discovery-specification-execution-pipeline.md|discovery-specification-execution-pipeline]]

---
_LLM 분석으로 생성됨_
