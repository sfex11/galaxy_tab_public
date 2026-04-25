# From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21910v1

## 💡 핵심 인사이트

과학 자동화의 진정한 병목은 계산적 실행이 아니라 인간 의도를 기계 실행 가능한 명세로 변환하는 의미론적 번역이며, 이를 해결하기 위해 해석과 생성을 분리한 3층 에이전트 아키텍처가 필요하다.

## 📖 분석

# From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation

## 핵심 문제: 의미론적 번역의 간극

기존 과학 워크플로우 시스템은 스케줄링, 장애 복구, 자원 관리 등 **실행(execution)**을 자동화하지만, 연구 질문을 워크플로우 명세로 변환하는 **의미론적 번역(semantic translation)**은 여전히 수동이다. 이 간극은 도메인 지식과 인프라 전문성을 동시에 요구하므로 자동화의 진정한 병목이다.

## 3층 에이전트 아키텍처

1. **의미론적 계층(Semantic Layer)**: LLM이 자연어 연구 질문을 구조화된 의도(intent)로 해석
2. **명세 생성 계층(Specification Layer)**: 검증된 생성기가 재현 가능한 워크플로우 명세를 생성
3. **실행 계층(Execution Layer)**: 기존 워크플로우 엔진과 연동

## Wiki 맥락에서의 위치

이 논문은 [[entities/scientific-workflow-agent|scientific-workflow-agent]]의 정의를 처음으로 구체화한다. 기존 [[entities/autoresearch|autoresearch]]가 문헌 탐색 수준의 자동화에 머물렀다면, 본 논문은 질문→명세→실행의 전체 파이프라인을 에이전트 아키텍처로 실현한다. [[concepts/discovery-specification-execution-pipeline|discovery-specification-execution-pipeline]] 개념의 실제 구현 사례이기도 하다.

[[sources/2026-04-23-chat2workflow-a-benchmark-for-generating-executabl.md|Chat2Workflow]]가 시각적 워크플로우 생성에 집중했다면, 본 논문은 **과학적 연구 질문**이라는 더 추상적인 입력에서 출발한다는 차이가 있다. [[sources/2026-04-10-syntax-is-easy-semantics-is-hard-evaluating-llms-f.md|Syntax Is Easy, Semantics Is Hard]]가 LTL 번역에서 구문은 쉽지만 의미는 어렵다고 지적한 것과 병렬적으로, 워크플로우 번역에서도 의미론적 변환의 난이도가 구문론적 변환을 압도함을 확인한다.

## 🔗 관련 논문

- 2026 04 23 chat2workflow a benchmark for generating executabl
- 2026 04 10 syntax is easy semantics is hard evaluating llms f

## 🏷️ 엔티티

- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]

## 📐 개념

- [[concepts/semantic-translation-gap.md|semantic-translation-gap]]
- [[concepts/three-layer-agentic-workflow.md|three-layer-agentic-workflow]]
- [[concepts/intent-structured-specification.md|intent-structured-specification]]

---
_LLM 분석으로 생성됨_
