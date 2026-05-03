# WorldDB: A Vector Graph-of-Worlds Memory Engine with Ontology-Aware Write-Time Reconciliation

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-22  
**링크**: http://arxiv.org/abs/2604.18478v1

## 핵심 요약

Persistent memory is the bottleneck separating stateless chatbots from long-running agentic systems. Retrieval-augmented generation (RAG) over flat vector stores fragments facts into chunks, loses cross-session identity, and has no first-class notion of supersession or contradiction. Recent bitemporal knowledge-graph systems (Graphiti, Memento, Hydra DB) add typed edges and valid-time metadata, but the graph itself remains flat: no recursive composition, no content-addressed invariants on nodes,...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

_없음_

## 추출된 개념

_없음_

## 메모

_자동 생성됨_

---
**관련**: [[concepts/write-time-reconciliation.md|write time reconciliation]]

## 🔗 교차 참조

- → [[sources/2026-04-24-automatic-ontology-construction-using-llms-as-an-e]]: 둘 다 평평한 벡터 기반 RAG의 메모리 파편화 한계를 지적하며, 하나는 그래프-오브-월드 구조로, 다른 하나는 RDF/OWL 형식 온톨로지로 구조적 지식 표현을 통해 이를 해결한다.
- → [[sources/2026-04-22-mass-rag-multi-agent-synthesis-retrieval-augmented]]: 둘 다 기존 평면적 벡터 RAG의 한계를 극복하려 하며, 하나는 다중 에이전트 합성으로 노이즈 문맥을 조정하고, 다른 하나는 구조화된 그래프 메모리로 단편화와 모순 문제를 해결한다.

---
**관련**: [[concepts/stateless-moderation.md|stateless moderation]]
