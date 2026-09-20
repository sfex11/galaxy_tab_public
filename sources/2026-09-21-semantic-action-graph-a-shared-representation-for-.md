# Semantic Action Graph: A Shared Representation for Agent Grounding and Human Interpretation of Sports Highlights

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20768v1

## 💡 핵심 인사이트

에이전트 그라운딩과 인간 검증·조향이 동일한 경량 도메인 스키마 위에서 동시에 성립할 때, 표현 설계가 인터페이스 설계에 선행하는 1급 문제가 된다.

## 📖 분석

본 논문은 하이라이트 생성 에이전트가 프레임 수준 비구조 표현 위에서 작동할 때 산출물 검증과 선호 조향이 불가능하다는 문제를 진단하고, 이를 '공유 표현' 설계로 해결한다. 경기를 수행자·행동·수신자·순간·상태 노드와 역할·시간·결과 엣지로 구성된 경량 도메인 스키마로 형식화하여, 동일 그래프가 에이전트의 그라운딩 매체이자 인간의 해석·감사·조향 매체로 이중 기능함을 세 속성(그라운딩, 검증가능성, 조향가능성)으로 확정한다.

[[dual-readership-interface]](Affora의 인터페이스 계층)의 원리가 표현 계층에서 실현되며, 이중 독자성이 부가 인터페이스가 아닌 스키마 내장 속성임을 입증한다. [[representation-contract]]의 당사자가 에이전트 간에서 에이전트-인간으로 확장되어, 계약 이행의 기준이 '읽을 수 있음'에서 '검증할 수 있음'으로 강화된다. [[verifiable-state-judging]] 관점에서 검증 단위가 출력 전체에서 노드·엣지 단위 상태 판독으로 세분화되고, [[preference-steerability]]는 그래프 요소 단위 선호 적용으로 조작화된다. [[cot-as-translated-report]]가 경고한 '번역된 보고서의 신뢰 문제'에 대해 내레이션의 구조적 근거를 제공하여, 에이전트 출력 감사([[interpretability-as-audit-layer]])를 블랙박스 신뢰에서 그래프 감사로 전환한다. v1 공식 발행으로 이 스키마가 표현 설계를 인터페이스 설계에 선행시키는 1급 문제임이 확정된다.

## 🔗 관련 논문

- Semantic Action Graph: A Shared Representation for Agent Gro
- Affora: A Design System for Agent-Friendly Interfaces
- Show-Harness: Just a VLM Agent Can Play Robots

## 🏷️ 엔티티

- [[entities/semantic-action-graph.md|semantic-action-graph]]
- [[entities/dual-readership-interface.md|dual-readership-interface]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/verifiable-state-judging.md|verifiable-state-judging]]
- [[entities/preference-steerability.md|preference-steerability]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/interpretability-as-audit-layer.md|interpretability-as-audit-layer]]
- [[entities/structured-intermediate-representation.md|structured-intermediate-representation]]

## 📐 개념

- [[concepts/semantic-action-graph.md|semantic-action-graph]]
- [[concepts/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[concepts/dual-readership-interface.md|dual-readership-interface]]
- [[concepts/verifiable-state-judging.md|verifiable-state-judging]]
- [[concepts/preference-steerability.md|preference-steerability]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/temporal-structure-loss-from-token-subsampling.md|temporal-structure-loss-from-token-subsampling]]
- [[concepts/interpretability-as-audit-layer.md|interpretability-as-audit-layer]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]

---
_LLM 분석으로 생성됨_
