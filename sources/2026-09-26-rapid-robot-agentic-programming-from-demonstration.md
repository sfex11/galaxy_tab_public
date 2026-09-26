# RAPID: Robot Agentic Programming from Demonstrations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30249v1

## 💡 핵심 인사이트

인간 시연은 모방할 데이터가 아니라 검증 가능한 명세이며, 코딩 에이전트의 테스트 주도 정제 루프가 이를 로봇 프로그램으로 컴파일한다.

## 📖 분석

RAPID는 단일 시각적 인간 시연에서 코딩 에이전트가 로봇 프로그램을 자동 생성·검증·정제하는 시스템이다. 핵심 구성은 (i) 검증 가능한 태스크 명세, (ii) 실행용 액션 프리미티브, (iii) 중간 표현이며, 반복적 생성-검증-정제 에이전틱 루프가 시연을 실행 가능한 코드로 컴파일한다.

[[harness-methodology-embodiment-migration]] 축의 결정적 사례다. TANDEM이 계획 중 필요 시점의 시연 수집([[as-needed-demonstration]])을 제안한 직후, RAPID는 단일 시연으로 전체 프로그램을 유도하여 시연 소비의 제3 경로를 연다 — 시연-컨텍스트([[demonstration-as-context]]), 시연-훈련데이터(모방 학습)에 이어 시연-명세(컴파일 대상)다. 시연이 모방의 데이터가 아니라 검증 가능한 명세로 재정의되는 전환이다.

[[test-encoded-behavioral-target]] 관점에서 검증 가능한 태스크 명세가 로봇 행동 정제의 실행 오라클로 작동함을 실증한다. ExecCritic 계열의 테스트 주도 개선 루프가 물리 도메인으로 확장되어, 코드 정확성뿐 아니라 로봇 행동도 테스트로 인코딩 가능함이 입증된다.

[[code-as-agent-harness]] 관점에서는 코드 생성의 명세 원천이 인간 프롬프트에서 시각 시연으로 확장됨을 보여주며, [[structured-intermediate-representation]]이 시연 이해와 코드 생성 사이의 번역 매개로 기능한다. [[obstacle-aware-harness]]가 안전 제약의 구조적 강제였다면 RAPID는 태스크 성공의 검증 기반 확보라는 짝 축을 제공한다.

## 🔗 관련 논문

- TANDEM: Task and Motion Planning with As-Needed Demonstratio
- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulati
- In-Context Robot Learning with VLM Agents
- ExecCritic: Learn to Test, Test to Improve for Codin

## 🏷️ 엔티티

- [[entities/rapid.md|rapid]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/demonstration-as-specification.md|demonstration-as-specification]]
- [[entities/as-needed-demonstration.md|as-needed-demonstration]]
- [[entities/demonstration-burden-automation.md|demonstration-burden-automation]]
- [[entities/demonstration-as-context.md|demonstration-as-context]]
- [[entities/test-encoded-behavioral-target.md|test-encoded-behavioral-target]]
- [[entities/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[entities/execution-verification.md|execution-verification]]

## 📐 개념

- [[concepts/demonstration-as-specification.md|demonstration-as-specification]]
- [[concepts/test-driven-robot-program-refinement.md|test-driven-robot-program-refinement]]

---
_LLM 분석으로 생성됨_
