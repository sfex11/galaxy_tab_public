# Semantic Action Graph: A Shared Representation for Agent Grounding and Human Interpretation of Sports Highlights

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20768v1

## 💡 핵심 인사이트

경량 도메인 스키마 하나가 에이전트의 그라운딩과 인간의 검증·조향을 동시에 담당하면, 에이전트 출력의 검증 가능성이 출력 자체의 신뢰가 아니라 공유 표현의 구조적 속성이 된다.

## 📖 분석

Semantic Action Graph(SAG)는 스포츠 경기를 행위자·행동·수신자·순간·상태 노드와 역할·시간·결과 엣지로 구성된 경량 도메인 스키마로 표현하여, 생성 에이전트의 하이라이트 선택·내레이션에 그라운딩을 제공한다. 핵심은 이 표현이 에이전트 그라운딩과 인간의 검증·선호 조향을 단일 매체로 동시에 서빙한다는 점이다. [[concepts/dual-readership-interface.md|dual readership interface]]가 인터페이스 계층에서 이중 독자 설계를 제시했다면, SAG는 동일 원리를 표현 계층으로 이동시켜 공유 표현 자체가 계약이 됨을 보인다. [[concepts/representation-contract.md|representation contract]] 관점에서, 프레임 수준·비구조 표현이 잃는 시간적·관계적 구조를 그래프가 명시 보존하여 에이전트 출력의 근거층이 된다. 이는 [[concepts/semantic-action-unit.md|semantic action unit]]의 단위 수준 계약을 노드-엣지 관계 구조로 확장하는 것이며, 내레이션이 번역물이라는 진단([[concepts/cot-as-translated-report.md|cot as translated report]])에 대해 그래프 감사라는 검증 경로를 제공해 [[concepts/interpretability-as-audit-layer.md|interpretability as audit layer]]의 구체 사례가 된다. 시청자가 출력을 검증하고 선호로 조향할 수 있다는 점은 [[concepts/preference-discovery-construction-boundary.md|preference discovery construction boundary]]의 인간 측 대응물이며, 검증 단위의 세분화는 [[entities/verifiable-state-judging.md|verifiable state judging]]을 시청자 도메인으로 확장한다.

## 🔗 관련 논문

- 2026-09-18-affora-a-design-system-for-agent-friendly-interfac.md
- 2026-09-11-show-harness-just-a-vlm-agent-can-play-robots.md

## 🏷️ 엔티티

- [[entities/semantic-action-graph.md|semantic-action-graph]]
- [[entities/dual-readership-interface.md|dual-readership-interface]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/semantic-action-unit.md|semantic-action-unit]]
- [[entities/interpretability-as-audit-layer.md|interpretability-as-audit-layer]]
- [[entities/verifiable-state-judging.md|verifiable-state-judging]]
- [[entities/temporal-structure-loss-from-token-subsampling.md|temporal-structure-loss-from-token-subsampling]]

## 📐 개념

- [[concepts/lightweight-domain-schema.md|lightweight-domain-schema]]
- [[concepts/preference-steerability.md|preference-steerability]]
- [[concepts/structured-intermediate-representation.md|structured-intermediate-representation]]

---
_LLM 분석으로 생성됨_
