# SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04167v1

## 💡 핵심 인사이트

기능 테스트 통과는 소프트웨어 엔지니어링 에이전트의 실세계 수용을 보장하지 않으며, 리뷰 파생 제약 준수라는 평가 누락 축이 벤치마크 점수와 실제 개발 기여도 사이의 구조적 단절을 만든다.

## 📖 분석

# SWE-Gate

**SWE-Gate**는 기존 저장소 수준 소프트웨어 엔지니어링 벤치마크가 기능 테스트 통과만을 측정하며, 실세계 패치 수용을 좌우하는 리뷰 파생 수용 제약(review constraints)을 간과한다는 진단에서 출발해, 리뷰 제약 준수를 명시적 평가 축으로 도입한 최초의 벤치마크다.

## Wiki 지형에서의 위치

- [[coverage-functionality-gap]]의 확장: RESTestBench가 '커버리지가 기능적 검증 적합성을 측정하지 못한다'는 간극을 제시했다면, SWE-Gate는 '테스트 통과가 수용 가능성을 측정하지 못한다'는 동형 논리를 패치 평가로 확장한다.
- [[benchmark-specification-gap]]의 구체 사례: 평가 단위(기능 테스트)와 배포 수용 단위(리뷰된 패치)의 불일치가 [[evaluation-deployment-unit-mismatch]]를 형성한다.
- [[evaluator-assumption]] 폭로: '테스트 통과 = 수용'이라는 암묵적 가정이 점수와 실세계 유용성을 단절시킨다.
- [[swe-chat]]과의 보완: SWE-chat이 야생 상호작용에서 태스크-현실 간극([[task-reality-divergence]])을 보였다면, SWE-Gate는 평가 계약 자체가 수용 워크플로우를 누락함을 보인다.

## 핵심 인사이트

인간 개발자의 패치가 테스트를 통과해도 리뷰에서 거절되듯, 에이전트 패치도 리뷰 문화·아키텍처 관례·유지보수성 요구라는 암묵적 계약을 충족해야 한다. 이 계약은 코드에 존재하지 않는 [[repository-operational-knowledge]]이며, 이를 측정하지 않는 벤치마크 점수는 실세계 기여도와 무관한 지표로 전락한다.

## 🔗 관련 논문

- RESTestBench: A Benchmark for Evaluating the Effectiveness o
- SWE-chat: Coding Agent Interactions From Real Users in the W
- ClassEval-Pro: A Cross-Domain Benchmark for Class-Level Code

## 🏷️ 엔티티

- [[entities/swe-gate.md|swe-gate]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[entities/coverage-functionality-gap.md|coverage-functionality-gap]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]
- [[entities/swe-chat.md|swe-chat]]
- [[entities/benchmark.md|benchmark]]
- [[entities/restestbench.md|restestbench]]

## 📐 개념

- [[concepts/review-constraint-compliance.md|review-constraint-compliance]]
- [[concepts/repository-operational-knowledge.md|repository-operational-knowledge]]
- [[concepts/task-reality-divergence.md|task-reality-divergence]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/benchmark-format-blindspot.md|benchmark-format-blindspot]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 생성됨_
