# SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04167v1

## 💡 핵심 인사이트

코딩 에이전트의 진정한 수용 기준은 기능 테스트 통과가 아니라 리뷰 제약 준수이며, 기존 SWE 벤치마크의 평가 프록시는 실제 배포 관문과 구조적으로 단절되어 있다 — SWE-Gate는 이 평가-배포 단위 불일치를 측정 가능한 벤치마크 차원으로 최초로 형식화했다.

## 📖 분석

SWE-Gate는 저장소 수준 소프트웨어 엔지니어링 벤치마크가 기능 테스트 통과라는 단일 프록시에 의존하며, 실제 패치 수용을 좌우하는 리뷰 기반 수용 제약(review constraints)을 간과한다는 문제 진단에서 출발한다. 리뷰 제약 준수를 명시적 평가 차원으로 채택한 최초의 저장소 수준 벤치마크로, 기능적 정확성과 수용 가능성 사이의 간극을 측정 가능하게 만든다.

Wiki 관점에서 본 논문은 세 층위로 기여한다. 첫째, [[evaluation-deployment-unit-mismatch]]에 '코드 리뷰 문화'라는 도메인 특정 차원을 추가한다 — 테스트 통과라는 평가 단위와 리뷰 승인이라는 배포 수용 단위의 불일치가 실제 개발에서 체계적으로 발생함을 실증한다. 둘째, [[restestbench]]의 [[coverage-functionality-gap]]과 동형 구조를 형성한다 — 측정 프록시와 실제 목표의 단절이 소프트웨어 평가의 범용적 결함임을 교차 검증한다. 셋째, [[review-constraint-compliance]]를 통해 리뷰 제약이 [[repository-operational-knowledge]]의 외면화된 형태임을 보여준다 — 프로젝트의 암묵적 규범이 리뷰 제약으로 형식화되는 것은 [[tacit-criteria-surfacing]]의 SWE 도메인 발현이다.

[[llm-as-code-reviewer]] 관점에서 SWE-Gate는 코드 리뷰 능력이 별도의 평가 축임을 정당화한다. 코딩 에이전트는 코드 의미론을 넘어 커뮤니티 규범을 모델링해야 하며, 이는 [[swe-chat]]이 제기한 [[task-reality-divergence]] 문제를 벤치마크 설계 수준에서 해소하는 경로가 된다.

## 🔗 관련 논문

- RESTestBench: A Benchmark for Evaluating the Effectiveness o
- SWE-chat: Coding Agent Interactions From Real Users in the W
- Beyond Summaries: Structure-Aware Labeling of Code Changes w

## 🏷️ 엔티티

- [[entities/swe-gate.md|swe-gate]]
- [[entities/review-constraint-compliance.md|review-constraint-compliance]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[entities/coverage-functionality-gap.md|coverage-functionality-gap]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]
- [[entities/repository-operational-knowledge.md|repository-operational-knowledge]]
- [[entities/llm-as-code-reviewer.md|llm-as-code-reviewer]]
- [[entities/task-reality-divergence.md|task-reality-divergence]]

## 📐 개념

- [[concepts/review-constraint-compliance.md|review-constraint-compliance]]
- [[concepts/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[concepts/coverage-functionality-gap.md|coverage-functionality-gap]]
- [[concepts/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[concepts/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/task-reality-divergence.md|task-reality-divergence]]

---
_LLM 분석으로 생성됨_
