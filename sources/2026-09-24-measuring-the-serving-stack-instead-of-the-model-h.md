# Measuring the Serving Stack Instead of the Model: Hidden Confounds in Local Tool-Use Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26693v1

## 💡 핵심 인사이트

로컬 서빙 스택의 정적 템플릿 게이팅이 도구 호출 가능성 자체를 결정하므로, 도구 사용 벤치마크 점수는 모델 능력이 아니라 모델-서빙 쌍의 속성으로 해석되어야 한다.

## 📖 분석

로컬 서빙 스택(Ollama 등)이 코딩 에이전트의 도구 호출 프로토콜 단계에 개입하는 방식을 규명한다. Ollama의 기본 `tools=` 요청이 정적 템플릿 플래그로 모델별 게이팅됨이 핵심 발견이다 — 일부 모델은 도구 정의를 받아 호출을 텍스트로 반환하고, 일부는 네이티브 tool_calls를 반환하며, Phi-3·Gemma-3는 정의 자체가 전달되지 않는다. 로컬 환경에서 측정된 도구 사용 성능은 모델 능력과 서빙 구성의 혼재물이 된다.

[[serving-layer-neutrality-premise]] 기각에 평가 측 증거를 추가한다. 스코어 센터링 연구가 훈련 신호(TIM)에서 서빙 비중립성을 보였다면, 본 논문은 도구 사용 평가에서 동일 전제가 무너짐을 보여 [[same-request-same-reading-assumption]]과 [[measurement-repeatability]]의 성립 조건을 서빙 구성 고정으로 명시한다.

[[elicitation-as-harness-artifact]]의 정교화다 — 템플릿 플래그라는 최소 설계 선택이 '모델이 도구를 쓸 수 있는가' 판정 자체를 좌우하므로, 도구 사용 능력은 모델 내재 속성이 아니라 모델-서빙 쌍의 속성이며 [[model-agnostic-harness]]의 반례가 된다. [[benchmark-specification-gap]] 관점에서 서빙 구성은 명세되지 않은 은닉 차원이며 [[harness-as-hidden-variable]]의 서빙 버전이다. 스키마가 도달하지 않는 실패는 [[schema-accumulation-bottleneck]]과 달리 도달 이전 단계의 병목이며, [[training-grade-serving-class]]와 병렬로 평가 등급 서빙 클래스의 필요성을 연다.

## 🔗 관련 논문

- An Empirical Study of Harness Design for Coding Agents
- Score Centering Stabilizes Off-policy Reinforcement Learning
- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading
- Clean Engineering, Unstable Measurement: A Preregistered Reliability Framework
- Pythia: Toward Predictability-Driven Agent-Native LLM Serving
- Testing Interchangeability in LLM Agent Teams

## 🏷️ 엔티티

- [[entities/serving-layer-neutrality-premise.md|serving-layer-neutrality-premise]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/tool-use.md|tool-use]]
- [[entities/model-agnostic-harness.md|model-agnostic-harness]]
- [[entities/same-request-same-reading-assumption.md|same-request-same-reading-assumption]]
- [[entities/elicitation-as-harness-artifact.md|elicitation-as-harness-artifact]]
- [[entities/model-harness-decomposability.md|model-harness-decomposability]]
- [[entities/detector-as-instrument.md|detector-as-instrument]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]

## 📐 개념

- [[concepts/training-grade-serving-class.md|training-grade-serving-class]]
- [[concepts/serving-stack-tool-gating.md|serving-stack-tool-gating]]
- [[concepts/measurement-repeatability.md|measurement-repeatability]]
- [[concepts/schema-accumulation-bottleneck.md|schema-accumulation-bottleneck]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-24-swe-serve-benchmarking-agentic-engineering-for-pro]]: 서빙 스택이 도구 사용 결과를 좌우한다는 문제의식을 공유하며, 한쪽은 이를 로컬 평가의 교란 변수로 규명하고 다른 한쪽은 이를 에이전트 엔지니어링의 새로운 벤치마크 도메인으로 격상시킨다.
- → [[sources/2026-09-25-can-llms-reason-about-runtime-behavior-a-repositor]]: 정적·선언적 평가의 한계를 지적하고, 서빙 스택의 실제 개입과 런타임 실행 같은 동적 행위를 직접 관찰해야 한다는 실행 기반 평가 방법론을 공유한다.
- → [[sources/2026-09-24-metrics-failure-in-llm-based-code-vulnerability-re]]: 평가 점수에 숨은 교란 변수(서빙 스택 게이팅, 포화된 컴파일률)가 모델 능력 신호를 오염시킴을 실증하는 평가 타당성 연구로 연결된다.
- → [[sources/2026-09-23-whose-facts-count-a-culturally-responsive-audit-of]]: 벤치마크 점수가 모델 능력이 아니라 평가 인프라(문화적 편향, 서빙 스택 게이팅)의 속성에 조건부임을 보이는 평가 도구 감사라는 관점을 공유한다.
