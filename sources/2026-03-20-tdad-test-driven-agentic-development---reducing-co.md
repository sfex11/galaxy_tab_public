# TDAD: Test-Driven Agentic Development - Reducing Code Regressions in AI Coding Agents via Graph-Based Impact Analysis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.17973v1

## 💡 핵심 인사이트

AI 코딩 에이전트의 성능 평가에서 '해결률'만이 아닌 '회귀 방지율'을 함께 측정해야 하며, AST 기반 코드-테스트 의존성 그래프가 이를 효과적으로 가능하게 한다.

## 📖 분석

## TDAD: Test-Driven Agentic Development

TDAD는 AI 코딩 에이전트가 실제 소프트웨어 이슈를 해결할 때 발생하는 **코드 회귀(regression)** 문제를 줄이기 위한 오픈소스 도구이자 벤치마크 방법론이다. 현재 SWE-bench 등 주요 벤치마크가 해결률(resolution rate)에만 집중하는 반면, TDAD는 기존에 통과하던 테스트가 깨지는 회귀 행동을 체계적으로 분석한다.

### 핵심 접근법

TDAD는 **AST(Abstract Syntax Tree) 기반 코드-테스트 그래프**를 구축하고, **가중 영향도 분석(weighted impact analysis)**을 통해 코드 변경에 의해 영향받을 가능성이 높은 테스트를 우선적으로 식별한다. 이는 전통적 소프트웨어 공학의 테스트 주도 개발(TDD) 원칙을 에이전트 개발 맥락으로 확장한 것이다.

### 기존 Wiki와의 관계

- **[[LLM Agent]]**: TDAD는 LLM 기반 코딩 에이전트의 신뢰성을 높이는 도구로, 에이전트가 코드를 수정할 때 의도치 않은 부작용을 사전에 탐지한다. 에이전트 평가의 새로운 차원(회귀 방지)을 제시한다는 점에서 [[claw-eval]], [[ace-bench]]와 같은 에이전트 평가 연구와 맥을 같이 한다.
- **[[ai-safety]]**: 코딩 에이전트의 안전한 배포를 위해 회귀 테스트는 필수적이며, TraceSafe가 다룬 가드레일 문제와 상보적 관계에 있다.
- **코드 리뷰 자동화**: CodeReviewAgentBenchmark와 연결되며, 코드 변경의 품질 보증 관점에서 상호 보완적이다.

### 의의

기존 벤치마크의 맹점(해결률만 측정)을 지적하고, 그래프 기반 정적 분석과 에이전트를 결합한 실용적 프레임워크를 제안했다는 점에서 AI 코딩 에이전트 분야의 성숙도를 높이는 연구다.

## 🔗 관련 논문

- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 09 ace bench agent configurable evaluation with scala
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- CodeReviewAgentBenchmark-slides.html
- 2026 04 09 gym anything turn any software into an agent envir

## 🏷️ 엔티티

- [[entities/llm-agent.md|LLM Agent]]

## 📐 개념

- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
