# RAPID: Robot Agentic Programming from Demonstrations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30249v1

## 💡 핵심 인사이트

시연을 테스트 가능한 명세로 컴파일하면 코딩 에이전트의 생성-검증-개선 루프가 물리 세계의 로봇 프로그램 획득으로 이식되며, 검증의 근거가 언어적 자기 평가가 아닌 로봇 실행이라는 외부 오라클로 이동한다.

## 📖 분석

RAPID는 코딩 에이전트의 코드 합성 역량을 로봇 시스템에 이식한다. 단일 시각적 인간 시연만을 입력으로 받아 로봇 프로그램을 자동 생성·검증·개선하는 반복적 에이전틱 루프를 제시한다. 이 루프가 성립하려면 세 가지 요소가 필요하다: (i) 테스트 가능한 태스크 명세, (ii) 로봇 실행용 액션 프리미티브, (iii) 시연 이해와 코드 생성 사이의 중간 표현.

이 논문은 [[harness-methodology-embodiment-migration]] 축의 핵심 착지점이다. 동일 시기의 Coding Agents for Generalized TAMP가 '도메인 엔지니어링을 수행하는 코드'로 이식한다면, RAPID는 '로봇 프로그램 자체'를 합성 대상으로 삼아 이식의 범위를 확정한다. Show-Harness가 VLM 에이전트의 직접 제어 경로를 보였다면, RAPID는 코드 생성 제어 경로의 유효성을 물리 도메인에서 실증하여 [[code-as-agent-harness]]를 확장한다.

핵심 구조적 발견은 시연의 위상 전환이다. 시연은 관찰 자료가 아니라 [[demonstration-as-specification]] — 테스트 가능한 명세로 컴파일되는 원천이다. 이 명세가 [[test-encoded-behavioral-target]]으로 인코딩되면 코드 개선 루프의 판정 기준이 되고, 테스트 주도 정제가 성립한다. TANDEM이 시연을 필요 시점에 요구하는 대안이라면, RAPID는 단일 시연의 명세화를 통한 자립적 프로그램 획득을 보여준다.

검증 루프는 로봇 실제 실행 결과에서 신호를 획득하며, 이는 LLM의 언어적 자기 평가가 아닌 물리 환경이라는 외부 오라클이 코드 정제의 근거가 됨을 의미한다 — [[execution-verification]]과 [[verification-as-system-external-relation]] 원리의 물리 도메인 실현이다.

## 🔗 관련 논문

- Coding Agents for Generalized Task and Motion Planning Problems
- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation
- Show-Harness: Just a VLM Agent Can Play Robots
- TANDEM: Task and Motion Planning with As-Needed Demonstrations
- RAPID: Robot Agentic Programming from Demonstrations

## 🏷️ 엔티티

- [[entities/rapid.md|rapid]]
- [[entities/demonstration-as-specification.md|demonstration-as-specification]]
- [[entities/test-encoded-behavioral-target.md|test-encoded-behavioral-target]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]

## 📐 개념

- [[concepts/test-driven-robot-program-refinement.md|test-driven-robot-program-refinement]]
- [[concepts/structured-intermediate-representation.md|structured-intermediate-representation]]
- [[concepts/execution-verification.md|execution-verification]]
- [[concepts/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[concepts/as-needed-demonstration.md|as-needed-demonstration]]

---
_LLM 분석으로 생성됨_
