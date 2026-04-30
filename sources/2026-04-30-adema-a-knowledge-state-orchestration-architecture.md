# ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge Synthesis with LLMAgents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25849v1

## 💡 핵심 인사이트

장기 지식 종합의 실패 원인은 단일 응답의 부정확성이 아니라 라운드 간 지식 상태의 은밀한 이동(drift)이며, 이를 해결하기 위해 지식 상태 자체를 일급 객체로 추적하는 인식론적 장부 기록이 필요하다.

## 📖 분석

# ADEMA: Knowledge-State Orchestration Architecture

**카테고리**: AI/ML — 에이전트 아키텍처
**생성일**: 2026-04-30

## 정의

ADEMA는 장기 지식 종합(long-horizon knowledge synthesis)을 위해 지식 상태(knowledge state)를 명시적으로 조율하는 에이전트 아키텍처다. 범용 다중 에이전트 런타임이 아닌, 지식 상태의 일관성을 유지하는 것 자체를 1차 목표로 설계되었다.

## 핵심 메커니즘

1. **인식론적 장부 기록(Epistemic Bookkeeping)**: 라운드 간 지식 상태를 명시적으로 추적하여 암묵적 중간 합약(implicit intermediate commitment)을 표면화
2. **이질적 이중 평가자 거버넌스**: 단일 평가자가 아닌 이질적 평가자 쌍이 지식 상태의 무결성을 검증
3. **적응적 태스크 모듈화**: 중단 후 재개 시 파단된 증거 연결(evidence chain)을 재구성

## 기존 Wiki와의 관계

이 아키텍처는 [[entities/epistemic-infrastructure|epistemic-infrastructure]]의 거버넌스·동기화·신뢰 계층을 구체적인 실행 아키텍처로 구현한다. 기존에 '구조화되어야 한다'고만 기술되던 인식론적 인프라에 대해, ADEMA는 지식 상태를 일급 객체(first-class object)로 취급하는 구체적 엔지니어링 경로를 제공한다.

[[entities/memory-management|memory-management]] 엔티티에 대해, ADEMA는 메모리를 단순한 아카이브가 아닌 지식 상태의 연속성을 보장하는 인식론적 장부로 재정의한다. [[concepts/memory-fragmentation-failure|memory-fragmentation-failure]]이 지적한 세션 간 일관성 파괴 문제에 대한 구조적 해법을 제시한다.

[[entities/autoresearch|autoresearch]]와의 관계에서, ADEMA는 [[concepts/storytelling-tax|storytelling-tax]]가 지적한 산출물 형태의 근본적 한계를 해결하지는 못하지만, 최소한 종합 과정 내부의 지식 상태 일관성을 보장하여 손실 압축이 '의도적 압축'이 아닌 '통제되지 않은 누출'이 되는 것을 방지한다.

## 관련 논문

- [[sources/2026-04-30-adema-a-knowledge-state-orchestration-architecture-fo.md|ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge Synthesis with LLM Agents]]

## 🔗 관련 논문

- 2026-04-27-from-research-question-to-scientific-workflow-leve
- 2026-04-24-automatic-ontology-construction-using-llms-as-an-e
- 2026-04-26-bilevel-autoresearch-meta-autoresearching-itself

## 🏷️ 엔티티

- [[entities/adema.md|adema]]
- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[entities/epistemic-bookkeeping.md|epistemic-bookkeeping]]
- [[entities/knowledge-state-drift.md|knowledge-state-drift]]
- [[entities/epistemic-infrastructure.md|epistemic-infrastructure]]
- [[entities/memory-management.md|memory-management]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/dual-evaluator-governance.md|dual-evaluator-governance]]

## 📐 개념

- [[concepts/knowledge-state-drift.md|knowledge-state-drift]]
- [[concepts/epistemic-bookkeeping.md|epistemic-bookkeeping]]
- [[concepts/evidence-chain-fracture.md|evidence-chain-fracture]]
- [[concepts/intermediate-commitment-tracking.md|intermediate-commitment-tracking]]
- [[concepts/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[concepts/dual-evaluator-governance.md|dual-evaluator-governance]]
- [[concepts/memory-fragmentation-failure.md|memory-fragmentation-failure]]
- [[concepts/epistemic-fidelity.md|epistemic-fidelity]]

---
_LLM 분석으로 생성됨_
