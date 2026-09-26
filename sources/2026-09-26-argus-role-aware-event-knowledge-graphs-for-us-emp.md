# ARGUS: Role-Aware Event Knowledge Graphs for U.S. Employment-Discrimination Complaints

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30184v1

## 💡 핵심 인사이트

이벤트 그래프 구축의 신뢰성은 범용 스키마가 아니라 수직 도메인의 역할 인식 스키마(5W1H)와 소스 근거 구속의 결합에서 나온다.

## 📖 분석

ARGUS는 CourtListener 고용차별 소송 문서에서 문서 수준 이벤트 지식 그래프(EKG)를 구축하는 소스 근거 파이프라인이다. 5W1H 기반 역할 인식 스키마, 법률 도메인 모델, LLM 구조화 생성을 결합해 사실 진술을 추출하고, 참여자·시간·인과 엣지를 갖는 청크 수준 이벤트 그래프를 문서 수준으로 통합한다.

기존 [[text-graph-fusion]] 계열([[event-extraction]])은 개방 도메인의 행위자-이벤트-객체 모델링이었으나, 본 논문은 법률 판례라는 수직 도메인으로의 정착 사례를 제공한다. [[llm-as-graph-refiner]]가 임상 EEG 그래프의 위양성 엣지 '제거'였다면, ARGUS는 원문 진술로부터 이벤트 구조를 '생성'하는 반대 방향으로, LLM-그래프 결합 패턴이 정제와 생성 양축으로 분화함을 보여준다.

[[semantic-action-graph]]와도 공통 원리를 공유한다 — 역할을 일급 요소로 명시하는 경량 스키마가 에이전트 그라운딩과 법률 문서 이해 양쪽에서 유효하다는 점에서 역할 인식 중간 표현의 도메인 불변성이 시사된다. source-grounded 설계는 [[evidence-traceability]]의 구현 사례로, 추출 사실의 원문 추적 가능성이 법률 도메인에서 그래프 신뢰성의 전제임을 확인시킨다. EKG는 비정형 법률 텍스트를 검색·추론이 소비할 수 있는 [[structured-intermediate-representation]]으로 격상시키는 후속 경로를 연다.

## 🔗 관련 논문

- A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extraction
- LLM as Clinical Graph Structure Refiner: Enhancing Representation Learning
- Semantic Action Graph: A Shared Representation for Agent Grounding and Human Verification
- Verifiable by Construction: Claim-Level Evaluation of Verbatim Citations

## 🏷️ 엔티티

- [[entities/event-extraction.md|event-extraction]]
- [[entities/text-graph-fusion.md|text-graph-fusion]]
- [[entities/llm-as-graph-refiner.md|llm-as-graph-refiner]]
- [[entities/evidence-traceability.md|evidence-traceability]]
- [[entities/semantic-action-graph.md|semantic-action-graph]]
- [[entities/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[entities/event-knowledge-graph.md|event-knowledge-graph]]
- [[entities/legal-domain-extraction.md|legal-domain-extraction]]

## 📐 개념

- [[concepts/event-knowledge-graph.md|event-knowledge-graph]]
- [[concepts/role-aware-event-schema.md|role-aware-event-schema]]
- [[concepts/source-grounded-extraction.md|source-grounded-extraction]]
- [[concepts/chunk-level-graph-aggregation.md|chunk-level-graph-aggregation]]

---
_LLM 분석으로 생성됨_
