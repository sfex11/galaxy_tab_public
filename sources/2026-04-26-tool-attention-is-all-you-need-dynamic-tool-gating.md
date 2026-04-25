# Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading for Eliminating the MCP/Tools Tax in Scalable Agentic Workflows

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21816v1

## 💡 핵심 인사이트

에이전트 워크플로우의 확장성 병목은 모델 능력이 아닌 상태 없는 도구 프로토콜의 스키마 주입 전략에 의해 발생하며, 동적 게이팅과 지연 로딩으로 이를 원천 차단할 수 있다.

## 📖 분석

# Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading

## MCP Tax의 정량화와 구조적 진단

본 논문은 Model Context Protocol(MCP)이 도구 증강 에이전트 워크플로우에 부과하는 숨겨진 오버헤드를 **MCP Tax**(10k~60k 토큰/턴)로 처음 정량화한다. 이 오버헤드의 근원은 상태 없는(stateless) 아키텍처에서 매 턴마다 전체 스키마를 주입하는 eager schema injection 방식이다.

## 도구 주의 메커니즘

제안하는 **Tool Attention**은 두 가지 축으로 작동한다: (1) 쿼리 관련성에 기반한 **동적 도어 게이팅**(불필요한 도구의 스키마를 사전에 차단)과 (2) 실제 호출 결정 시점에만 스키마를 로드하는 **Lazy Schema Loading**. 이는 기존 Wiki에서 식별된 [[stateless-architecture-vulnerability|상태 없는 아키텍처 취약점]]을 도구 선택 맥락 상실이라는 구체적 실패 모드로 실증하며, [[context-fracture-point|컨텍스트 파단점]] 부근에서의 추론 품질 저하를 완화한다.

## 기존 Wiki와의 연결

- [[swe-chat]] 분석에서 "MCP Tax를 제어 변수로 포함해야 함"을 시사했던 부분에 대한 직접적 해답 제공
- [[token-step-pipeline-hierarchy|토큰→스텝→파이프라인 최적화 계층]]에서 토큰 수준 최적화의 구체적 구현 사례
- [[serving-safety-coupling|서빙-안전성 커플링]]의 토큰 오버헤드 축 — 스키마 팽창이 KV 캐시를 압박하여 가드레일 적용 가능성을 간접적으로 제한
- [[transient-turn-injection]]이 노출한 다중 턴 취약점과 동일 근원(상태 없는 아키텍처)을 공유하되, 안전성이 아닌 효율성 축에서 해결

## 🔗 관련 논문

- 2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md
- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md
- 2026-04-25-transient-turn-injection-exposing-stateless-multi-.md

## 🏷️ 엔티티

- [[entities/tool-attention.md|tool-attention]]
- [[entities/model-context-protocol.md|model-context-protocol]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/aggregate-pipeline-serving.md|aggregate-pipeline-serving]]
- [[entities/swe-chat.md|swe-chat]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/mcp-tax.md|mcp-tax]]
- [[concepts/tools-tax.md|tools-tax]]
- [[concepts/dynamic-tool-gating.md|dynamic-tool-gating]]
- [[concepts/lazy-schema-loading.md|lazy-schema-loading]]
- [[concepts/eager-schema-injection.md|eager-schema-injection]]
- [[concepts/context-fracture-point.md|context-fracture-point]]
- [[concepts/tool-context-optimization.md|tool-context-optimization]]
- [[concepts/stateless-architecture-vulnerability.md|stateless-architecture-vulnerability]]

---
_LLM 분석으로 생성됨_
