# Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading for Eliminating the MCP/Tools Tax in Scalable Agentic Workflows

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21816v1

## 💡 핵심 인사이트

도구 스키마의 eager injection은 단순한 토큰 낭비가 아니라 문맥 활용도의 파단점에 도달하여 추론 품질을 구조적으로 저하시키는 숨겨된 부하(MCP Tax)이며, 이를 Tool Attention 기반 동적 게이팅으로 해소해야 에이전트 워크플로우가 실제 스케일에서 작동한다.

## 📖 분석

# Tool Attention Is All You Need: MCP/Tools Tax의 발견과 해소

## MCP Tax의 구조적 발견

Model Context Protocol(MCP)이 도구 연결의 표준으로 자리잡았지만, 본 논문은 stateless eager schema injection이 초래하는 숨겨진 부하 — **MCP Tax(Tools Tax)** — 를 최초로 정량화한다. 다중 서버 배포에서 턴당 10k~60k 토큰에 달하는 이 부하는 단순한 비용 문제가 아니다. KV-Cache를 팽창시켜 서빙 메모리 압박을 가중하고, 문맥 활용도가 기존에 보고된 '파단점(fracture points)'에 근접할 때 **추론 품질 저하**를 유발한다는 점에서 [[concepts/kv-cache-optimization|KV-Cache 최적화]]와 [[concepts/reasoning-shift|추론 시프트]]의 교차점에 위치한다.

## 동적 도구 게이팅과 지연 스키마 로딩

제안된 **Tool Attention** 메커니즘은 두 축으로 구성된다: (1) 현재 질의와 관련성이 높은 도구만 활성화하는 **동적 도어 게이팅**, (2) 실제 호출 시점까지 스키마 로딩을 지연시키는 **지연 스키마 로딩**. 이는 [[concepts/token-step-pipeline-hierarchy|토큰→스텝→파이프라인 최적화 계층]]에서 파이프라인 수준의 최적화를 도구 인터페이스 계층으로 확장한다.

## 기존 Wiki와의 연결

[[concepts/aggregate-pipeline-serving|Aggregate Pipeline Serving]]이 다중 LLM 호출의 집합적 최적화를 다룬다면, 본 논문은 그 파이프라인에 주입되는 **도구 스키마라는 또 다른 부하 축**을 식별한다. [[concepts/dynamic-context-injection|동적 컨텍스트 주입]]의 Indexer→Selector→Injector 패턴과 본질적으로 동일한 철학 — 필요한 것만 선택적으로 주입 — 을 도구 인터페이스에 적용한 것으로 볼 수 있다.

[[entities/swe-chat|SWE-chat]]이나 [[entities/computer-use-agent|컴퓨터 사용 에이전트]]의 실제 배포 환경에서 MCP Tax는 샌드박스 벤치마크에서는 측정되지 않는 숨겨진 성능 저하因子다. [[concepts/sandbox-liveworld-gap|샌드박스-실세계 격차]]의 새로운 기여 요인으로 기능할 가능성이 높다.

## 🔗 관련 논문

- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md
- 2026-04-23-chat2workflow-a-benchmark-for-generating-executabl.md

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/aggregate-pipeline-serving.md|aggregate-pipeline-serving]]
- [[entities/swe-chat.md|swe-chat]]
- [[entities/model-context-protocol.md|model-context-protocol]]
- [[entities/tool-attention.md|tool-attention]]

## 📐 개념

- [[concepts/mcp-tax.md|mcp-tax]]
- [[concepts/tools-tax.md|tools-tax]]
- [[concepts/tool-attention.md|tool-attention]]
- [[concepts/dynamic-tool-gating.md|dynamic-tool-gating]]
- [[concepts/lazy-schema-loading.md|lazy-schema-loading]]
- [[concepts/eager-schema-injection.md|eager-schema-injection]]
- [[concepts/context-fracture-point.md|context-fracture-point]]
- [[concepts/tool-context-optimization.md|tool-context-optimization]]

---
_LLM 분석으로 생성됨_
