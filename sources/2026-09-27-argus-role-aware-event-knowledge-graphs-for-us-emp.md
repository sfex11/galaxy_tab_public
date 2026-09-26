# ARGUS: Role-Aware Event Knowledge Graphs for U.S. Employment-Discrimination Complaints

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30184v1

## 💡 핵심 인사이트

어휘·임베딩 표현으로는 포착 불가능한 법적 복합 사건 서열이 5W1H 역할 스키마의 소스 접지형 사건 그래프로 표현 가능함을 보여주며, LLM의 역할을 그래프 정제에서 소스 접지된 그래프 생성으로 확장한다.

## 📖 분석

ARGUS는 CourtListener 고용차별 소송 문서에서 문서 수준 Event Knowledge Graph(EKG)를 구축하는 소스-접지 파이프라인이다. 사실 진술을 추출하고 5W1H 기반 역할 스키마로 청크 수준 사건 그래프(참여자·시간·인과)를 만든 뒤 문서 단위로 집계한다.

핵심 진단은 표현의 한계에 있다: 어휘·임베딩 표현만으로는 법적 소송의 복합 사건 서열을 포착할 수 없다. 이는 open-domain 사건 추출([[event-extraction]])이 검색·관계 모델링을 다룬 것과 달리, 법 도메인에서 구조적 사건 표현이 사실 표현 자체의 문제임을 규정한다.

LLM 역할의 흥미로운 대칭이 드러난다: [[llm-as-graph-refiner]]가 생체신호(EEG) 그래프의 위상을 '정제'하는 데 LLM을 썼다면, ARGUS는 텍스트로부터 그래프를 '생성'하는 데 법률 도메인 모델과 LLM 구조화 생성을 결합한다. LLM의 그래프 지식 파이프라인 관여가 정제→생성으로 확장되는 흐름이다.

청크→문서 집계는 [[structured-intermediate-representation]]의 실현 사례이며, 소스 접지성은 [[evidence-traceability]] 논의(사후 진단·인용 검증 계열)와 연결된다. EKG가 법률 QA와 [[graph-rag]]의 근거 구조로 기능할 가능성을 연다.

## 🔗 관련 논문

- ARGUS: Role-Aware Event Knowledge Graphs for U.S. Employment
- LLM as Clinical Graph Structure Refiner: Enhancing Representation Lear
- A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extr
- Large Language Models (LLMs) for Telecom Root Cause Analysis

## 🏷️ 엔티티

- [[entities/event-knowledge-graph.md|event-knowledge-graph]]
- [[entities/legal-domain-extraction.md|legal-domain-extraction]]
- [[entities/role-aware-event-schema.md|role-aware-event-schema]]
- [[entities/chunk-level-graph-aggregation.md|chunk-level-graph-aggregation]]
- [[entities/source-grounded-extraction.md|source-grounded-extraction]]
- [[entities/llm-as-graph-refiner.md|llm-as-graph-refiner]]

## 📐 개념

- [[concepts/event-extraction.md|event-extraction]]
- [[concepts/text-graph-fusion.md|text-graph-fusion]]
- [[concepts/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[concepts/graph-rag.md|graph-rag]]
- [[concepts/evidence-traceability.md|evidence-traceability]]
- [[concepts/structured-knowledge-extraction.md|structured-knowledge-extraction]]

---
_LLM 분석으로 생성됨_
