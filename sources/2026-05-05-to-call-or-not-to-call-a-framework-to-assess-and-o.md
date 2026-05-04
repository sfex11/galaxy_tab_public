# To Call or Not to Call: A Framework to Assess and Optimize LLM Tool Calling

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00737v1

## 💡 핵심 인사이트

도구 호출의 최적화는 비용 최소화가 아니라 호출/미호출 결정 경계에서의 정확도 최대화 문제이며, 외부 정보는 항상 이익이 아니라 내부 지식과의 상호작용에 따라 해가 될 수 있다.

## 📖 분석

## 도구 호출의 이중성: 비용 절감을 넘어선 해로성 문제

기존 Wiki는 도구 사용의 비용 측면—MCP Tax([[tools-tax]]), 스키마 축적 병목([[schema-accumulation-bottleneck]]), 지연 스키마 로딩([[lazy-schema-loading]])—에 집중해 왔다. 본 논문은 이 비용 중심 프레임을 '도구 호출의 해로성(harmfulness)'이라는 새로운 축으로 확장한다. 웹 검색 도구에서 모델 내부 지식으로 충분한 질문에 외부 도구를 호출하면 오히려 정확도가 하락할 수 있으며, 이는 [[token-efficiency]] 최적화가 항상 성능 향상과 정렬되지 않음을 보여준다.

이는 [[blind-tool-invocation]] 문제에 대한 체계적 평가 프레임워크를 최초로 제공한다는 점에서 의의가 있다. 기존 [[tool-attention]]이 '어떤 도구에 주의를 기울일 것인가'를 다루었다면, 본 논문은 '도구에 주의를 기울여야 하는가 자체'를 결정 문제로 형식화한다.

[[aggregate-pipeline-serving]]의 관점에서 보면, 불필요한 도구 호출은 레이턴시뿐 아니라 검색 결과의 노이즈가 파이프라인 하류에 복합적으로 전파되는 구조적 위험을 창출한다. [[cost-dominance-dimension-asymmetry]]의 비용 축(인프라)이 해로성 축(행동 품질)과 결합하는 새로운 비대칭을 드러낸다. 또한 이 결정은 본질적으로 [[metacognition]]—자신이 무엇을 아는지에 대한 인지—를 요구하며, [[adaptive-inference]]가 단순한 연산량 조절이 아닌 인지적 자기 평가를 포함해야 함을 시사한다.

## 🔗 관련 논문

- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo
- Pythia: Toward Predictability-Driven Agent-Native LLM Serving

## 🏷️ 엔티티

- [[entities/tool-use.md|tool-use]]
- [[entities/blind-tool-invocation.md|blind-tool-invocation]]
- [[entities/tool-attention.md|tool-attention]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/aggregate-pipeline-serving.md|aggregate-pipeline-serving]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/metacognition.md|metacognition]]
- [[entities/cost-dominance-dimension-asymmetry.md|cost-dominance-dimension-asymmetry]]
- [[entities/tools-tax.md|tools-tax]]

## 📐 개념

- [[concepts/redundant-tool-calling.md|redundant-tool-calling]]
- [[concepts/tool-calling-harmfulness.md|tool-calling-harmfulness]]
- [[concepts/knowledge-tool-substitution-boundary.md|knowledge-tool-substitution-boundary]]

---
_LLM 분석으로 생성됨_
