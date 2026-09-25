# A2M: Trace-Optimized Agent Hijacking in the MCP Ecosystem

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26761v1

## 💡 핵심 인사이트

시맨틱 매칭으로 도구를 선택하는 에이전트 능력 자체가 공급망 공격 표면이며, 실행 트레이스가 공격자의 최적화 피드백으로 전용될 수 있음을 보여준다.

## 📖 분석

A2M은 MCP 생태계에서 에이전트의 도구 선택이 의존하는 시맨틱 매칭 자체를 공격 벡터로 전환하는 이중 단계 블랙박스 하이재킹 프레임워크를 제시한다. Attraction 단계는 공격자 제어 도구 메타데이터를 최적화해 호출 확률을 극대화하고, Manipulation 단계는 실행 트레이스를 피드백으로 활용해 적대적 도구 반환값을 점진 정교화한다.

기존 Wiki에 대한 핵심 기여는 세 가지다. 첫째, [[schema-accumulation-attack-surface]]가 수동적 정보 누출을 다뤘다면 본 논문은 스키마 주입을 능동적 공격 최적화 대상으로 격상시킨다 — 메타데이터가 오버헤드이자 공격 벡터의 이중성을 실증한다. 둘째, [[trace-as-attack-surface]]에 제3의 역할을 추가한다: 트레이스가 관측 매체·피감시자 생성물이라는 이중성에 공격자의 최적화 피드백 신호라는 차원을 더한다. 셋째, [[efficiency-attack-surface-identity]]의 MCP 도메인 실증이다 — 시맨틱 매칭이라는 효율 메커니즘이 곧 공격 표면이라는 명제가 구체적 공격 프레임워크로 구현된다.

[[capability-safety-inseparability]] 관점에서 시맨틱 매칭을 제거하면 에이전트 능력도 소멸하므로 방어는 능력 축소가 아닌 도구 출처 인증·메타데이터 무결성 검증 같은 구조적 계층에서 이루어져야 한다. 이는 [[zero-trust-agent-architecture]]에 구체적 위협 모델을 제공하며, [[mcp-tax]]의 오버헤드-보안 긴장을 새 차원으로 확장한다.

## 🔗 관련 논문

- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading
- The Natural Language Interaction Protocol and Standard for AI Agents
- Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities

## 🏷️ 엔티티

- [[entities/model-context-protocol.md|model-context-protocol]]
- [[entities/mcp-tax.md|mcp-tax]]
- [[entities/schema-accumulation-attack-surface.md|schema-accumulation-attack-surface]]
- [[entities/trace-as-attack-surface.md|trace-as-attack-surface]]
- [[entities/efficiency-attack-surface-identity.md|efficiency-attack-surface-identity]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/blind-tool-invocation.md|blind-tool-invocation]]
- [[entities/zero-trust-agent-architecture.md|zero-trust-agent-architecture]]
- [[entities/eager-schema-injection.md|eager-schema-injection]]
- [[entities/history-anchors.md|history-anchors]]
- [[entities/agent-native-immune-system.md|agent-native-immune-system]]
- [[entities/semantic-supply-chain.md|semantic-supply-chain]]
- [[entities/trace-optimized-attack.md|trace-optimized-attack]]

## 📐 개념

- [[concepts/semantic-supply-chain.md|semantic-supply-chain]]
- [[concepts/trace-optimized-attack.md|trace-optimized-attack]]
- [[concepts/tool-metadata-poisoning.md|tool-metadata-poisoning]]
- [[concepts/black-box-agent-hijacking.md|black-box-agent-hijacking]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-23-onpanda-efficient-annotation-of-on-policy-alignmen]]: 에이전트 실행 궤적을 핵심 객체로 다룬다는 점에서 연결되며, onPanda의 궤적 주석·교정은 A2M 유형 하이재킹 궤적의 탐지·정제를 위한 방어 측 데이터 기반을 제공할 수 있다.
- → [[sources/2026-09-23-rare-event-estimation-via-iterative-unalignment]]: 자율 에이전트 배포가 만드는 안전 위협을 다루되, 한쪽은 능동적 공격 벡터(MCP 하이재킹)를, 다른 한쪽은 희귀 재난 이벤트의 발생 확률 추정을 다루는 에이전트 안전 연구로 연결된다.
