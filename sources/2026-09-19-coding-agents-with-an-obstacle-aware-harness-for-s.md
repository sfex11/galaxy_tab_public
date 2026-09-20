# Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20822v1

## 💡 핵심 인사이트

안전 제약이 에이전트 컨텍스트에 가시화되지 않으면 코딩 에이전트는 목표 추구에만 최적화되어 물리적 안전을 침해하므로, 로봇 조작 안전의 병목은 모델 능력이 아니라 하네스의 제약 표현 설계에 있다.

## 📖 분석

코딩 에이전트가 로봇 제어기를 프로그램으로 작성하는 패러다임에 최초로 안전 평가 축을 도입한다. 각 태스크에 조작 목표와 금지 접촉 장애물을 쌍으로 부과하자 에이전트는 대부분 목표만 추구하며 충돌한다 — 안전 제약이 에이전트 컨텍스트에 가시화되지 않으면 사실상 존재하지 않는다는 진단이다.

이는 [[concepts/planning-without-physical-constraint-encoding.md|planning without physical constraint encoding]]의 실증적 확장이다. 안전 여백 등 물리적 제약이 LLM 계획에 내재화되지 않는다는 진단이 자연어 계획에서 코드 생성 경로로 재현되어, 도메인 불변 구조 결함임을 강화한다. 해법은 모델 능력 향상이 아니라 장애물을 입력 계약에 명시하는 장애물 인지 하네스이며, [[concepts/harness-side-compensation.md|harness side compensation]]의 로보틱스 실현이다 — [[entities/sentinel-rl.md|sentinel rl]]이 위상 추론을 그래프로 오프로딩했다면 본 논문은 안전 제약의 가시화를 하네스로 오프로딩한다.

[[entities/show-harness.md|show harness]]와 컨텍스트 로봇 학습이 VLM 직접 제어 경로를 다뤘다면 본 논문은 코드 생성 제어 경로의 안전을 평가하여, 이종 제어 경로가 '안전 제약의 가시화'라는 동일 병목으로 수렴함을 보여준다. [[concepts/capability-safety-inseparability.md|capability safety inseparability]] 관점에서 조작 능력과 충돌 회피의 분리 실패가 프롬프트 신호 비대칭 수준에서 재현되며, [[concepts/representation-contract.md|representation contract]] 관점에서 안전 제약의 표현 형식이 행동을 규정하는 하네스-에이전트 계약임을 시사한다.

## 🔗 관련 논문

- Show-Harness: Just a VLM Agent Can Play Robots
- In-Context Robot Learning with VLM Agents
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the S
- Affora: A Design System for Agent-Friendly Interfaces

## 🏷️ 엔티티

- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/obstacle-aware-harness.md|obstacle-aware-harness]]
- [[entities/planning-without-physical-constraint-encoding.md|planning-without-physical-constraint-encoding]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/safety-critical-control.md|safety-critical-control]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/show-harness.md|show-harness]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]

## 📐 개념

- [[concepts/safety-constraint-context-legibility.md|safety-constraint-context-legibility]]
- [[concepts/goal-safety-signal-asymmetry.md|goal-safety-signal-asymmetry]]

---
_LLM 분석으로 생성됨_
