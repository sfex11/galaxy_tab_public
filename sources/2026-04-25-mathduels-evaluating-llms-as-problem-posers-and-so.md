# MathDuels: Evaluating LLMs as Problem Posers and Solvers

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21916v1

## 💡 핵심 인사이트

정적 벤치마크에서의 천장 성능 문제는 더 어려운 문제를 만드는 것이 아니라, 모델 스스로 문제를 출제하고 푸는 셀프플레이 구조를 통해 평가의 차별력을 동적으로 확보함으로써 해결된다.

## 📖 분석

# MathDuels

**카테고리**: 벤치마크
**생성일**: 2026-04-25

## 정의

MathDuels는 LLM이 문제 출제자와 해결자의 이중 역할을 동시에 수행하는 셀프플레이 기반 수학 벤치마크다. 각 모델이 적대적 프롬프팅 하에 수학 문제를 출제하고, 동시에 다른 모든 참가 모델이 출제한 문제를 푸는 3단계 생성 파이프라인을 통해 문제를 생산한다.

## 기존 벤치마크와의 구조적 차이

기존 Wiki에서 [[benchmark]] 엔티티가 추적해온 벤치마크 위기 — RoboGrid의 "구문·행동·의미 혼재" 문제, SWE-chat의 "정적 태스크 한계" — 와 동일한 진단선 위에 있다. 정적 문제 집합에서 프론티어 모델이 천장 성능에 도달하면 벤치마크가 모델 간 차별력을 상실한다는 공통된 인식이다. MathDuels는 이를 **평가 대상(문제) 자체를 동적으로 생성**하는 방식으로 해결한다.

## 셀프플레이의 평가론적 의미

[[llm-as-judge]]가 지적한 LLM judge의 추이성 위반 문제와 대비된다. LLM-as-judge가 평가자의 비일관성에서 기인한다면, MathDuels의 셀프플레이는 **평가 대상의 동적성**으로 차별력을 확보한다. 문제 출제 능력 자체가 새로운 평가 축이 되며, 이는 [[adversarial-prompting]]을 문제 해결이 아닌 문제 생성에 전용하는 패러다임 전환이다.

## 관련 논문

- [[sources/2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-s.md|MathDuels: Evaluating LLMs as Problem Posers and Solvers]]

## 🔗 관련 논문

- 2026 04 24 diagnosing cfg interpretation in llms
- 2026 04 24 swe chat coding agent interactions from real users

## 🏷️ 엔티티

- [[entities/mathduels.md|mathduels]]
- [[entities/benchmark.md|benchmark]]
- [[entities/llm.md|llm]]
- [[entities/llm-benchmark.md|llm-benchmark]]

## 📐 개념

- [[concepts/self-play-benchmark.md|self-play-benchmark]]
- [[concepts/dual-role-evaluation.md|dual-role-evaluation]]
- [[concepts/adversarial-problem-generation.md|adversarial-problem-generation]]
- [[concepts/dynamic-benchmark.md|dynamic-benchmark]]
- [[concepts/problem-posing-evaluation.md|problem-posing-evaluation]]
- [[concepts/ceiling-performance-problem.md|ceiling-performance-problem]]

---
_LLM 분석으로 생성됨_
