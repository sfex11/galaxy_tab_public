# Automatic Ontology Construction Using LLMs as an External Layer of Memory, Verification, and Planning for Hybrid Intelligent Systems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20795v1

## 💡 핵심 인사이트

벡터 기반 RAG의 메모리 파편화 한계를 형식적 온톨로지(RDF/OWL)로 구조적으로 해결함으로써, LLM 에이전트의 지식이 비단순 검색 가능한 수준을 넘어 검증 가능하고 모순 없는 상태로 유지되는 인식론적 인프라의 실제 구현 경로를 제시한다.

## 📖 분석

# 자동 온톨로지 구축: LLM을 위한 외부 기억·검증·계획 층

## 핵심 주장
이 논문은 LLM이 매개변수적 지식과 벡터 기반 RAG에만 의존하는 구조적 한계를 지적하며, RDF/OWL 기반의 형식적 온톨로지를 외부 기억 층으로 구축하는 자동화 파이프라인을 제안한다. 벡터 스토어의 단순 청크 검색이 아닌, 의미적으로 구조화된 지식 그래프를 통해 지속적·검증 가능·의미론적으로 정합한 추론을 가능하게 한다.

## 기존 Wiki와의 관계

### 메모리 파편화 실패에 대한 구조적 대안
Wiki의 `memory-fragmentation-failure` 개념이 플랫 벡터 스토어가 세션 간 일관성과 모순 조정을 파괴한다고 진단한 것에 대해, 본 논문은 형식적 온톨로지(RDF/OWL)가 이를 해결하는 구조적 수단이 될 수 있음을 실증한다. 청크 단위 파편화를 개체-관계-제약의 구조적 표현으로 대체한다.

### 인식론적 인프라의 구현 경로
`epistemic-infrastructure` 엔티티가 지식의 확정 상태·신뢰 등급·쟁점 여부를 추적해야 한다고 주장한 것에 대해, 온톨로지는 이를 형식적으로 인코딩할 수 있는 표현 체계를 제공한다. OWL의 추론 기능은 모순 탐지를 내장적으로 수행한다.

### 쓰기 시점 조정의 구체화
`write-time-reconciliation`이 데이터 저장 시 온톨로지를 인식하여 일관성을 강제한다고 정의한 것에 대해, 본 논문의 자동 온톨로지 구축 파이프라인은 이를 실제로 구현하는 엔지니어링 경로다.

## 다른 논문과의 연결점
- Mass RAG(2026-04-22): 다중 에이전트 합성 검색이 구조적 지식 없이 파편화될 위험을 온톨로지가 완화 가능
- WorldDB(2026-04-22): 벡터-그래프 하이브리드 메모리 엔진과 본 논문의 방향성이 수렴하나, 본 논문은 형식적 의미론(Formal Semantics)을 추가로 요구
- PSI(2026-04-11): 공유 상태 버스가 온톨로지 계층을 기반으로 작동할 경우 일관성 보장이 강화됨

## 🔗 관련 논문

- 2026 04 22 mass rag multi agent synthesis retrieval augmented
- 2026 04 22 worlddb a vector graph of worlds memory engine wit
- 2026 04 11 psi shared state as the missing layer for coherent

## 🏷️ 엔티티

- [[entities/epistemic-infrastructure.md|epistemic-infrastructure]]
- [[entities/llm.md|llm]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/memory-management.md|memory-management]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/graph-rag.md|graph-rag]]

## 📐 개념

- [[concepts/ontology-construction.md|ontology-construction]]
- [[concepts/external-ontological-memory.md|external-ontological-memory]]
- [[concepts/rdf-owl-representation.md|rdf-owl-representation]]
- [[concepts/write-time-reconciliation.md|write-time-reconciliation]]
- [[concepts/memory-fragmentation-failure.md|memory-fragmentation-failure]]
- [[concepts/epistemic-fidelity.md|epistemic-fidelity]]
- [[concepts/formal-semantic-grounding.md|formal-semantic-grounding]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[concepts/unified-memory-pool.md|unified memory pool]]

---
**관련**: [[concepts/planning-without-physical-constraint-encoding.md|planning without physical constraint encoding]]

---
**관련**: [[concepts/hazard-avoidance-planning.md|hazard avoidance planning]]

---
**관련**: [[concepts/entropy-regularized-planning.md|entropy regularized planning]]

---
**관련**: [[concepts/cross-domain-memory-transfer.md|cross domain memory transfer]]

---
**관련**: [[concepts/repository-memory.md|repository memory]]

---
**관련**: [[concepts/self-organizing-systems.md|self organizing systems]]

---
**관련**: [[concepts/compensatory-memory-dynamics.md|compensatory memory dynamics]]

---
**관련**: [[concepts/proactive-safety-planning.md|proactive safety planning]]

## 🔗 교차 참조

- → [[sources/2026-04-22-worlddb-a-vector-graph-of-worlds-memory-engine-wit]]: 둘 다 평평한 벡터 기반 RAG의 메모리 파편화 한계를 지적하며, 하나는 그래프-오브-월드 구조로, 다른 하나는 RDF/OWL 형식 온톨로지로 구조적 지식 표현을 통해 이를 해결한다.

---
**관련**: [[entities/entropy-regularized-planning.md|entropy regularized planning]]

---
**관련**: [[concepts/step-level-verification-decoding.md|step level verification decoding]]

---
**관련**: [[concepts/memory-enhanced-debate.md|memory enhanced debate]]

---
**관련**: [[concepts/layer-wise-forgetting-sensitivity.md|layer wise forgetting sensitivity]]

---
**관련**: [[concepts/hierarchical-planning.md|hierarchical planning]]

---
**관련**: [[entities/proof-planning-depth.md|proof planning depth]]

---
**관련**: [[entities/hierarchical-planning.md|hierarchical planning]]

---
**관련**: [[entities/external-layer-principle.md|external layer principle]]

---
**관련**: [[concepts/evaluation-planning-irreducibility.md|evaluation planning irreducibility]]

---
**관련**: [[concepts/external-layer-principle.md|external layer principle]]

---
**관련**: [[concepts/global-local-planning-hierarchy.md|global local planning hierarchy]]

---
**관련**: [[concepts/runtime-verification-layer.md|runtime verification layer]]
