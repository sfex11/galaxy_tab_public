# MathDuels: Evaluating LLMs as Problem Posers and Solvers

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21916v1

## 💡 핵심 인사이트

수학적 문제 해결 능력과 문제 출제 능력은 별개의 독립적 역량이며, 고정 벤치마크에서의 천장 성능은 모델 간 실제 역량 차이를 은폐할 뿐이다.

## 📖 분석

# MathDuels: Evaluating LLMs as Problem Posers and Solvers

## 기존 Wiki와의 관계

MathDuels는 기존 Wiki에서 이미 식별된 [[concepts/ceiling-performance-problem.md|천장 성능 문제]]에 대한 구체적 해법을 제시한다. 기존 [[concepts/llm-benchmark.md|LLM 벤치마크]] 엔티티에서 "고정된 문제 집합에서의 천장 성능"을 극복하는 접근법으로 언급되었으나, 본 논문은 이를 완전한 평가 프레임워크로 구현했다.

## 핵심 메커니즘

3단계 생성 파이프라인(기초 문제→난이도 상향→적대적 프롬프팅)을 통해 문제를 생성하고, 모든 참가 모델이 쌍방향으로 출제-해결을 수행하는 셀프플레이 구조다. 이는 [[concepts/evaluator-assumption.md|평가자의 가정]]을 구조적으로 해체한다—문제 공간이 사전 정의가 아닌 모델에 의해 동적 구성된다.

## 주요 발견: 출제-해결 비대칭성

[[concepts/dual-role-evaluation.md|이중 역할 평가]]가 드러낸 가장 중요한 인사이트는 해결 능력과 출제 능력이 별개의 역량이라는 점이다. 이는 [[concepts/safety-transfer-gap.md|안전성 전이 격차]]와 구조적으로 유사하다—한 평가 모달리티에서의 성능이 다른 모달리티로 자동 전이되지 않는 것처럼, 풀이 성능이 출제 성능을 보장하지 않는다.

## 다른 논문과의 연결

- [[sources/2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md|SWE-chat]]이 실제 사용 환경에서의 [[concepts/task-reality-divergence.md|태스크-현실 간극]]을 드러냈다면, MathDuels는 평가 설계 차원에서 이 간극의 원인(고정 문제 집합)을 제거한다.
- [[sources/2026-04-24-diagnosing-cfg-interpretation-in-llms.md|RoboGrid]]가 구문·행동·의미의 3축 분리를 제안했다면, MathDuels는 출제와 해결을 독립 축으로 분리하여 각각의 능력을 개별적으로 측정한다.

## 🔗 관련 논문

- 2026 04 24 swe chat coding agent interactions from real users
- 2026 04 24 diagnosing cfg interpretation in llms

## 🏷️ 엔티티

- [[entities/mathduels.md|mathduels]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[entities/dual-role-evaluation.md|dual-role-evaluation]]
- [[entities/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[entities/self-play-benchmark.md|self-play-benchmark]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/bidirectional-competency-asymmetry.md|bidirectional-competency-asymmetry]]
- [[concepts/dynamic-evaluation-landscape.md|dynamic-evaluation-landscape]]
- [[concepts/solver-poser-decoupling.md|solver-poser-decoupling]]

---
_LLM 분석으로 생성됨_
