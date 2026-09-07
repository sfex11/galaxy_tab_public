# Multi-Step Tool-Calling over Korean Open Public APIs: A Benchmark and a Data-Synthesis Recipe

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05395v1

## 💡 핵심 인사이트

오픈소스 LLM의 멀티스텝 도구 호출 열위는 아키텍처 한계가 아닌 훈련 데이터 간극이며, 실행에 근거한 동적 그래프 합성으로 해소 가능하다.

## 📖 분석

KOPA-Bench는 데이터 주권 규제로 온프레미스 오픈소스 배포가 강제되는 공공기관을 겨냥해, 한국 공공 개방 API 위에서 다단계 도구 호출을 수행하는 145개 실제 태스크로 구성된 벤치마크를 제시한다. 오픈소스 모델이 이 설정에서 일관되게 열위이며 기존 벤치마크가 이 간극을 측정하지 못한다는 진단에 따라, EDGE(Execution-grounded Dynamic Graph)라는 도구 호출 학습 데이터 합성 레시피를 함께 제안한다.

Wiki 지형에서의 위치: Claw-Eval-Live가 실세계 워크플로우 수요로 벤치마크 신호를 갱신했다면([[refreshable-signal-layer]]), KOPA-Bench는 라이브 정부 API를 표적으로 삼아 같은 원리를 공공 도메인에 구현한다. Tool Attention([[mcp-tax]])이 도구 스키마 오버헤드라는 인프라 병목을 드러냈다면, 본 논문은 병목의 다른 축인 오픈소스 모델의 멀티스텝 호출 능력 부족을 정량화한다. EDGE의 실행 근거 데이터 합성은 [[verifiable-training-data-synthesis]]의 구체적 실현이며, [[agent-environment-generation]]이 환경 생성에서 학습 데이터 합성으로 확장된 사례다. 데이터 주권이라는 규제 요인이 [[on-device-inference]]의 새로운 구동 축이 되고, 오픈소스 모델의 열위는 [[slm-reasoning-gap]]의 도구 호출 도메인 발현으로 읽힌다.

## 🔗 관련 논문

- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflo
- RESTestBench: A Benchmark for Evaluating the Effectiveness o
- Gym-Anything: Turn any Software into an Agent Environment

## 🏷️ 엔티티

- [[entities/kopa-bench.md|kopa-bench]]
- [[entities/edge-data-synthesis.md|edge-data-synthesis]]
- [[entities/tool-use.md|tool-use]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/mcp-tax.md|mcp-tax]]
- [[entities/synthetic-data-generation.md|synthetic-data-generation]]

## 📐 개념

- [[concepts/data-sovereignty.md|data-sovereignty]]
- [[concepts/execution-grounded-synthesis.md|execution-grounded-synthesis]]
- [[concepts/multi-step-tool-calling.md|multi-step-tool-calling]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/live-api-evaluation.md|live-api-evaluation]]

---
_LLM 분석으로 생성됨_
