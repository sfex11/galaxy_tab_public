# Coding Agents for Generalized Task and Motion Planning Problems

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30233v1

## 💡 핵심 인사이트

일반화 TAMP의 병목은 계획 자체가 아니라 인스턴스 간 정규성을 활용하는 도메인 엔지니어링이며, 이 엔지니어링까지 코딩 에이전트가 코드로 합성할 수 있다 — 에이전트의 산출물이 플랜이 아니라 플랜을 만드는 인프라라는 점이다.

## 📖 분석

이산 결정과 기하·기동·동역학 제약의 긴밀한 결합으로 TAMP가 어려운 가운데, 일반화 TAMP의 기존 방법들은 인스턴스 간 정규성을 활용하는 스트림·샘플러·매크로를 전문가가 수공업으로 구축해야 한다는 병목을 안고 있다. 본 논문은 이 도메인 엔지니어링 자체를 코딩 에이전트가 소수 예시 인스턴스로부터 코드로 합성할 수 있음을 실증한다.

Wiki 지형에서의 위치는 세 층위다. 첫째, [[concepts/coding-agent-for-domain-engineering.md|coding agent for domain engineering]]·[[concepts/generalized-tamp.md|generalized tamp]]의 원천 정의를 확립한다 — 에이전트의 산출물이 문제의 해(플랜)가 아니라 문제를 빨리 풀게 하는 인프라 코드라는 점에서, CodeMidas([[concepts/codebase-as-learning-environment.md|codebase as learning environment]])의 코드→학습환경 변환과 병렬되는 '인스턴스→일반화 코드' 변환 경로를 연다. 둘째, [[concepts/harness-methodology-embodiment-migration.md|harness methodology embodiment migration]]에 제3의 착지점을 부여한다 — 코딩 에이전트 방법론이 물리 계획 도메인으로 이식되되, 이식 대상이 제어기 코드(RAPID)나 안전 하네스([[concepts/obstacle-aware-harness.md|obstacle aware harness]])가 아닌 계획 기제 코드라는 점이 이식의 성격을 정교화한다. 셋째, [[concepts/domain-regularity-as-code.md|domain regularity as code]]의 원천 사례로서, 인스턴스 간 정규성이 암묵적 전문 지식이 아니라 합성·검증 가능한 명시적 코드로 현현할 수 있음을 보여준다.

TANDEM([[concepts/tamp-teleoperation-hybrid-data-collection.md|tamp teleoperation hybrid data collection]])이 시연 매개의 엔지니어링 경감이었다면 본 논문은 코드 합성 매개의 완전 자동화로, TAMP 특화 엔지니어링 부담 제거의 스펙트럼을 완성한다.

## 🔗 관련 논문

- Coding Agents for Generalized Task and Motion Planning Problems
- RAPID: Robot Agentic Programming from Demonstrations
- TANDEM: Task and Motion Planning with As-Needed Demonstrations
- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation

## 🏷️ 엔티티

- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]
- [[entities/coding-agent-for-domain-engineering.md|coding-agent-for-domain-engineering]]
- [[entities/generalized-tamp.md|generalized-tamp]]
- [[entities/domain-regularity-as-code.md|domain-regularity-as-code]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/codebase-as-learning-environment.md|codebase-as-learning-environment]]
- [[entities/obstacle-aware-harness.md|obstacle-aware-harness]]
- [[entities/tamp-teleoperation-hybrid-data-collection.md|tamp-teleoperation-hybrid-data-collection]]

## 📐 개념

- [[concepts/coding-agent-for-domain-engineering.md|coding-agent-for-domain-engineering]]
- [[concepts/generalized-tamp.md|generalized-tamp]]
- [[concepts/domain-regularity-as-code.md|domain-regularity-as-code]]
- [[concepts/code-as-agent-harness.md|code-as-agent-harness]]
- [[concepts/codebase-as-learning-environment.md|codebase-as-learning-environment]]
- [[concepts/obstacle-aware-harness.md|obstacle-aware-harness]]
- [[concepts/tamp-teleoperation-hybrid-data-collection.md|tamp-teleoperation-hybrid-data-collection]]

---
_LLM 분석으로 생성됨_
