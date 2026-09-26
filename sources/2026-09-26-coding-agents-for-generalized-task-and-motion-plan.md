# Coding Agents for Generalized Task and Motion Planning Problems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30233v1

## 💡 핵심 인사이트

TAMP 일반화의 병목은 계획 알고리즘이 아니라 도메인 규칙성을 명시화하는 특화 엔지니어링이며, 이 엔지니어링 자체를 코딩 에이전트의 코드 합성 대상으로 전환함으로써 LLM 능력이 물리 계획 도메인의 지식 축적 계층에 직접 기여할 수 있음을 보여준다.

## 📖 분석

본 논문은 코딩 에이전트가 일반화된 태스크·동작 계획(Generalized TAMP)의 도메인 특화 엔지니어링을 자동화할 수 있는지를 조사한다. TAMP의 근본 난제는 이산적 결정이 기하·운동학·동역학 제약과 강결합된다는 점이며, 기존 일반화 방법은 문제 인스턴스 간 규칙성을 활용하려면 상당한 TAMP 특화 엔지니어링을 요구했다. 본 논문은 이 수작업 엔지니어링 자체를 에이전트의 코드 합성 대상으로 전환한다는 점에서 의미가 있다.

기존 Wiki와의 관계에서 세 지점이 중요하다. 첫째, [[demonstration-burden-automation]]과 [[as-needed-demonstration]] 계열(tandem-task-and-motion-planning-with-as-needed-dem)이 TAMP에서 시연 부담을 줄이는 데 집중했다면, 본 논문은 엔지니어링 부담을 자동화 대상으로 격상시켜 TAMP 지원의 스펙트럼을 확장한다. 둘째, [[planning-without-physical-constraint-encoding]]과 [[goal-safety-signal-asymmetry]]가 지적한 'LLM 계획이 물리적 제약을 인코딩하지 못한다'는 진단을 전제로 하면서, 그 해법을 하네스 장애물 인코딩([[obstacle-aware-harness]])이 아닌 도메인별 제약 처리 코드의 합성에 둔다. 셋째, [[code-as-agent-harness]]와 [[code-as-evolution-unit]]의 원리가 코딩 도메인에서 물리적 계획 도메인으로 이식되는 사례로서, [[harness-methodology-embodiment-migration]]이 관찰한 코딩→로보틱스 방법론 이동의 추가 증거가 된다. 본질적으로 '도메인 규칙성을 코드로 명시화하는 작업'이 일반화의 핵심 병목임을 특정하며, 이는 [[algorithm-system-translation-gap]]의 물리 도메인 변형 — 도메인 지식을 기호적 코드 계층으로 번역하는 작업 — 으로 읽을 수 있다.

## 🔗 관련 논문

- 2026-09-25-tandem-task-and-motion-planning-with-as-needed-dem
- 2026-09-21-coding-agents-with-an-obstacle-aware-harness-for-s

## 🏷️ 엔티티

- [[entities/tandem-task-and-motion-planning-with-as-needed-dem.md|tandem-task-and-motion-planning-with-as-needed-dem]]
- [[entities/planning-without-physical-constraint-encoding.md|planning-without-physical-constraint-encoding]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]
- [[entities/code-as-evolution-unit.md|code-as-evolution-unit]]

## 📐 개념

- [[concepts/generalized-tamp.md|generalized-tamp]]
- [[concepts/coding-agent-for-domain-engineering.md|coding-agent-for-domain-engineering]]
- [[concepts/domain-regularity-as-code.md|domain-regularity-as-code]]

---
_LLM 분석으로 생성됨_
