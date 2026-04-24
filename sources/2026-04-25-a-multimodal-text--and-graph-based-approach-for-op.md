# A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extraction from Documents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21885v1

## 💡 핵심 인사이트

텍스트의 의미적 이해 능력과 그래프의 구조적 관계 모델링을 결합함으로써, 사전 정의 없이도 일반화 가능한 개방 도메인 이벤트 추출을 달성할 수 있다.

## 📖 분석

# 멀티모달 텍스트-그래프 기반 개방 도메인 이벤트 추출

## 기존 Wiki와의 관계

본 논문은 [[entities/graph-rag|Graph RAG]]의 그래프 구조화 원리를 이벤트 추출 도메인으로 전이한다. 기존 Graph RAG가 지식 검색을 위해 그래프를 활용한다면, 본 연구는 문서 내 이벤트의 구조적 관계(행위자-이벤트-객체)를 그래프로 명시적으로 모델링하여, 단순 텍스트 기반 추출의 한계를 극복한다.

## 핵심 기여: 폐쇄-개방 도메인 간극의 해소

기존 이벤트 추출 연구는 두 극단에 위치해 있었다: (1) 사전 정의된 이벤트 유형에 국한된 폐쇄 도메인 방식은 일반화가 불가능하며, (2) 개방 도메인 방식은 LLM의 잠재력을 충분히 활용하지 못했다. 본 논문은 텍스트(의미적 이해)와 그래프(구조적 관계)를 결합하여 이 간극을 해소한다.

## 인식론적 인프라와의 연결

[[entities/epistemic-infrastructure|인식론적 인프라]] 관점에서, 이벤트 추출은 비정형 텍스트를 구조화된 지식으로 변환하는 '인식론적 충실도'의 문제다. [[concepts/formal-fidelity-gap|형식적 일관성-인식론적 충실도 간극]] 개념과 직결되며, 그래프 기반 구조화가 이 간극을 좁히는 메커니즘으로 작동한다. 이는 [[concepts/write-time-reconciliation|쓰기 시점 조정]]과도 연결되는데, 추출 시점에 구조적 일관성을 강제하는 방식이기 때문이다.

## 다른 논문과의 연결

- [[sources/2026-04-24-automatic-ontology-construction-using-llms-as-an-e.md|Automatic Ontology Construction]]이 온톨로지를 정적 구조로 구축한다면, 본 논문은 이벤트를 동적으로 추출하여 지식 그래프를 실시간으로 확장한다.
- [[entities/llm|LLM]] 합성 분석에서 지적된 '안전성과 정렬' 축 외에, LLM이 구조화된 정보 추출에서 보여주는 신뢰성 문제도 동일한 추론 무결성 프레임워크로 분석 가능하다.

## 🔗 관련 논문

- 2026 04 24 automatic ontology construction using llms as an e

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/graph-rag.md|graph-rag]]
- [[entities/epistemic-infrastructure.md|epistemic-infrastructure]]
- [[entities/event-extraction.md|event-extraction]]

## 📐 개념

- [[concepts/event-extraction.md|event-extraction]]
- [[concepts/open-domain-event-extraction.md|open-domain-event-extraction]]
- [[concepts/multimodal-event-extraction.md|multimodal-event-extraction]]
- [[concepts/text-graph-fusion.md|text-graph-fusion]]
- [[concepts/structured-knowledge-extraction.md|structured-knowledge-extraction]]

---
_LLM 분석으로 생성됨_
