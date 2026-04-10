# TDAD: Test-Driven Agentic Development - Reducing Code Regressions in AI Coding Agents via Graph-Based Impact Analysis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17973v1

## 💡 핵심 인사이트

AI 코딩 에이전트의 평가는 해결률뿐 아니라 회귀 방지 능력까지 포함해야 하며, AST 기반 그래프 분석이 이를 체계적으로 측정하는 효과적인 방법이 될 수 있다.

## 📖 분석

## TDAD: Test-Driven Agentic Development

TDAD는 AI 코딩 에이전트가 실제 소프트웨어 이슈를 해결할 때 발생하는 **코드 회귀(regression)** 문제를 체계적으로 분석하고 줄이기 위한 오픈소스 도구이자 벤치마크 방법론이다. 현재 SWE-bench 등 주요 벤치마크가 해결률(resolution rate)에만 집중하는 반면, TDAD는 에이전트가 기존에 통과하던 테스트를 깨뜨리는 회귀 행동에 주목한다.

### 핵심 기술

TDAD는 **추상 구문 트리(AST) 기반 코드-테스트 그래프**를 구축하고, 가중 영향 분석(weighted impact analysis)을 통해 코드 변경에 의해 영향받을 가능성이 높은 테스트를 식별한다. 이는 전통적인 소프트웨어 공학의 테스트 주도 개발(TDD) 철학을 에이전트 개발 파이프라인에 접목한 것으로, 그래프 기반 정적 분석과 LLM 에이전트의 결합이 특징적이다.

### 연구 의의

이 연구는 AI 코딩 에이전트의 **신뢰성과 안전성** 평가에 새로운 차원을 추가한다. 단순히 문제를 풀 수 있는지가 아니라, 풀면서 다른 것을 망가뜨리지 않는지를 측정한다는 점에서 [[concepts/ai-safety|AI Safety]] 논의와 직결된다. 또한 [[entities/llm-agent|LLM Agent]]의 실용적 배포를 위해 회귀 방지가 필수적임을 실증적으로 보여준다.

### 관련 연구와의 연결

ACE-Bench(에이전트 평가 벤치마크), CLAW-Eval(자율 에이전트 신뢰성 평가)과 함께 LLM 에이전트의 평가 방법론을 다각화하는 흐름에 위치한다. EvaluatingLLM-BasedTestGeneration 연구와도 테스트 생성·활용 관점에서 상보적이다. CodeReviewAgentBenchmark와는 코드 품질 자동 평가라는 공통 관심사를 공유한다.

## 🔗 관련 논문

- 2026 04 09 ace bench agent configurable evaluation with scala
- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 chatbot based assessment of code understanding in

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
