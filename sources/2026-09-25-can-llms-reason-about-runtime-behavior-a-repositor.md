# Can LLMs Reason About Runtime Behavior? A Repository-Level Dynamic Benchmark

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28449v1

## 💡 핵심 인사이트

정적 코드 이해와 런타임 동작 추론은 별개의 능력이며, 저장소 규모의 동적 추론은 LLM 판정이 아닌 실행 오라클 기반 평가로만 신뢰성 있게 측정 가능하다.

## 📖 분석

SWE-Flux는 저장소 수준에서 정적 코드 이해가 아닌 동적 실행 추론을 평가하는 벤치마크로, 12개 실제 Python 저장소의 480개 실행 기반(execution-grounded) 인스턴스를 제공한다. 기존 저장소 수준 QA 벤치마크는 정적 이해와 LLM 판정 의존에 머물렀고, 실행 추론 벤치마크는 스니펫·함수 수준에 국한되어 있었다는 이중 간극을 채운다.

Wiki 관점에서 이 논문은 두 축의 교차점을 확정한다. [[repository-level-code-understanding]] 축(저장소 규모)과 [[execution-verification]] 축(실행 오라클)의 결합으로, [[rlvr]]의 검증 가능성 원리가 저장소 규모의 런타임 동역학 평가로 확장됨을 보여준다. [[meaning-insensitive-metric]]과 [[judge-instrument-reliability]]가 지적한 LLM 판정 불안정성에 대해 실행 기반 판정이라는 구조적 해법을 제시한다.

[[swe-serve]](서빙), [[vloc-bench]](보안)에 이어 실행 추론이라는 새 수직 도메인을 추가해 [[benchmark-domain-specialization]] 흐름을 강화하며, 정적 이해가 런타임 추론을 담보하지 않는 정적-동적 간극을 저장소 규모에서 측정 가능하게 만든다. [[codebase-as-learning-environment]] 관점에서 저장소가 코딩 RL 환경과 서빙 평가에 이어 동적 실행 추론 평가 인프라로도 재질화됨을 입증한다.

## 🔗 관련 논문

- SWE-Serve: Benchmarking Agentic Engineering For Production Inference S
- Vulnerability Localization Benchmark: Measuring Agentic Secu
- Metrics Failure in LLM-Based Code Vulnerability Repair: An E

## 🏷️ 엔티티

- [[entities/swe-flux.md|swe-flux]]
- [[entities/repository-level-code-understanding.md|repository-level-code-understanding]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/benchmark-domain-specialization.md|benchmark-domain-specialization]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/codebase-as-learning-environment.md|codebase-as-learning-environment]]
- [[entities/dynamic-execution-reasoning.md|dynamic-execution-reasoning]]
- [[entities/static-dynamic-reasoning-gap.md|static-dynamic-reasoning-gap]]

## 📐 개념

- [[concepts/dynamic-execution-reasoning.md|dynamic-execution-reasoning]]
- [[concepts/static-dynamic-reasoning-gap.md|static-dynamic-reasoning-gap]]

---
_LLM 분석으로 생성됨_
