# The SIMPLE Law for Energy Cost of LLM Inference

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03330v1

## 💡 핵심 인사이트

LLM 추론 에너지는 토큰 수의 선형 함수가 아니다 — 각 토큰이 KV 캐시에 진입해 이후 토큰의 비용을 구조적으로 상승시키므로, 비용은 시퀀스 위치의 비선형 함수이며 이를 per-LLM fit이 아닌 폐쇄형 해석 법칙으로 유도할 수 있다.

## 📖 분석

LLM 추론 에너지 비용에 대한 폐쇄형 해석 법칙(SIMPLE law)을 제시한다. 핵심 명제는 토큰이 동등하지 않다는 것 — 각 토큰이 KV 캐시에 진입하면 이후 토큰의 비용을 끌어올리므로, 표면적으로 동일한 토큰의 비용이 시퀀스 위치에 따라 비선형적으로 증가한다. SOTA 비용 모델이 아키텍처를 fitted coefficient로 흡수하는 per-LLM fit인 것과 대조적으로, 본 논문은 계산 복잡도와 메모리 접근 복잡도의 해석적 폐쇄형을 유도하여 fit이 아닌 law로서 아키텍처 무관 예측을 확립한다.

위키 맥락에서 이 법칙은 세 축에 근거를 공급한다. (1) 메커니즘 축: [[kv-cache-optimization]], [[kv-streams]], [[flash-dllm]]이 공략하는 캐시 병목의 비용론적 정당화 — 압축·퇴거의 가치가 절약 바이트가 아닌 차단된 비용 증가 사슬로 측정될 수 있음. (2) 에이전트 파이프라인 축: [[schema-accumulation-bottleneck]]과 [[retry-context-accumulation-loop]]의 비용 폭주가 휴리스틱 관찰이 아니라 법칙적 귀결임을 확정하고, [[behavior-infrastructure-dual-cost-model]]에 '시퀀스 위치 의존적 한계 비용' 차원을 추가한다. (3) 서빙 축: [[decode-phase-gemv-serving-cost]]의 경험적 비용이 해석적으로 유도 가능함을 보이며, [[token-consumption-forecasting]]의 예측에는 토큰 수를 비용으로 변환하는 법칙 기반 계층의 필요성이 부과된다.

## 🔗 관련 논문

- Flash-dLLM: IO-Aware KV Caching and Parallel Decoding for Fa
- TokenCast: Forecasting Token Consumption During LLM Agent Ex
- KV-streams for Efficient Compaction in Agentic Reinforcement
- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy
- On the Fundamental Limits of Prefill-Based Decoding Length P

## 🏷️ 엔티티

- [[entities/simple-law.md|simple-law]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/kv-streams.md|kv-streams]]
- [[entities/flash-dllm.md|flash-dllm]]
- [[entities/decode-phase-gemv-serving-cost.md|decode-phase-gemv-serving-cost]]
- [[entities/token-consumption-forecasting.md|token-consumption-forecasting]]
- [[entities/behavior-infrastructure-dual-cost-model.md|behavior-infrastructure-dual-cost-model]]
- [[entities/schema-accumulation-bottleneck.md|schema-accumulation-bottleneck]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/mcp-tax.md|mcp-tax]]

## 📐 개념

- [[concepts/simple-law.md|simple-law]]
- [[concepts/non-linear-token-cost.md|non-linear-token-cost]]
- [[concepts/kv-cache-marginal-cost.md|kv-cache-marginal-cost]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/kv-cache-optimization.md|kv-cache-optimization]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-05-you-dont-need-long-context]]: SIMPLE 법칙이 KV 캐시로 인해 후반 토큰 비용이 최대 7배까지 비선형 증가하는 구조를 폐쇄형으로 설명하여, 빈번한 컴팩션으로 짧은 컨텍스트를 유지하는 전략에 이론적 근거를 제공한다.
