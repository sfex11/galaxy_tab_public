# A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extraction from Documents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21885v1

## 💡 핵심 인사이트

이벤트 추출에서 그래프 구조는 검색의 보조 수단이 아니라 행위자-이벤트-객체 간 관계를 명시적으로 모델링하여 개방 도메인 일반화를 가능하게 하는 핵심 표현 형식이다.

## 📖 분석

# A Multimodal Text- and Graph-Based Approach for Open-Domain Event Extraction from Documents

**카테고리**: 정보 추출 · 그래프 기반 NLP
**날짜**: 2026-04-26

## 핵심 기여

기존 이벤트 추출이 사전 정의된 이벤트 유형(closed-domain)에 국한되어 일반화가 불가능했던 한계를, LLM 기반의 개방 도메인 접근법으로 극복한다. 핵심은 텍스트 처리와 그래프 구조를 융합하여 행위자-이벤트-객체 간 관계를 명시적으로 모델링하는 것으로, 단순히 이벤트를 '발견'하는 것을 넘어 이벤트 간 구조적 관계를 그래프로 표현한다.

## 기존 Wiki와의 관계

### graph-rag의 용도 확장
기존 Wiki에서 graph-rag가 '검색 증강' 도구로 묘사되던 것을, 본 논문은 '구조화된 정보 추출' 도구로 확장한다. 그래프가 문서 내 이벤트의 관계망을 명시적으로 표현하므로, 검색뿐 아니라 이벤트 클러스터링·인과 추론·문서 요약의 기반이 된다.

### 온톨로지 구축과의 연결
[[sources/2026-04-24-automatic-ontology-construction-using-llms-as-an-e.md|Automatic Ontology Construction]]이 지식의 거버넌스·신뢰 계층을 형식적으로 구현했다면, 본 논문은 그 하위에서 이벤트라는 구체적 지식 단위를 비형식적으로 추출하는 실용 경로를 제공한다. 두 논문의 결합이 인식론적 인프라의 실행 가능성을 높인다.

### epistemic-infrastructure로의 공급
추출된 이벤트 그래프는 인식론적 인프라의 입력으로 기능할 수 있으나, 본 논문이 다루는 개방 도메인 설정에서는 추출 결과의 신뢰 등급 부여 문제가 새로운 과제로 떠오른다.

## 🔗 관련 논문

- 2026-04-24-automatic-ontology-construction-using-llms-as-an-e.md
- 2026-04-24-worlddb-a-vector-graph-of-worlds-memory-engineine-wit

## 🏷️ 엔티티

- [[entities/event-extraction.md|event-extraction]]
- [[entities/graph-rag.md|graph-rag]]
- [[entities/text-graph-fusion.md|text-graph-fusion]]

## 📐 개념

- [[concepts/multimodal-event-extraction.md|multimodal-event-extraction]]
- [[concepts/open-domain-event-extraction.md|open-domain-event-extraction]]
- [[concepts/structured-knowledge-extraction.md|structured-knowledge-extraction]]

---
_LLM 분석으로 생성됨_
