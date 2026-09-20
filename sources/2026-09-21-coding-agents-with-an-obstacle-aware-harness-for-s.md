# Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20822v1

## 💡 핵심 인사이트

코딩 에이전트 기반 로봇 제어에서 안전은 모델 능력의 부산물이 아니라, 하네스가 장애물을 구조적 하드 제약으로 인코딩할 때에만 확보된다.

## 📖 분석

본 논문은 코딩 에이전트가 로봇 제어기를 프로그램으로 생성하는 패러다임의 안전성을 최초로 정량 평가한다. 조작 목표와 접촉 금지 장애물이 짝지어진 태스크에서 에이전트는 대부분 장애물과 충돌하며, 장애물을 회피해야 할 하드 제약이 아닌 소프트 고려사항으로 취급함을 실증한다. 이는 [[capability-safety-inseparability]]의 물리 도메인 결정적 사례다 — 목표 달성에 최적화된 코드 생성 능력은 안전을 산출하지 않으며, 능력과 안전의 구조적 분리가 코딩 에이전트에서도 성립함을 보여준다. 제안하는 [[obstacle-aware-harness]]는 [[goal-safety-signal-asymmetry]]의 처방을 제시한다: 목표 신호와 달리 안전 제약은 컨텍스트 서술만으로는 불충분하므로, [[safety-constraint-context-legibility]] 원칙에 따라 장애물을 하네스 계층의 일급 제약으로 인코딩하고 [[interpretive-vs-structural-enforcement]] 구도에서 구조적 강제 경로를 채택한다. 이는 [[planning-without-physical-constraint-encoding]] 진단의 실증적 확정이자 [[harness-side-compensation]]의 로보틱스 구현이다. [[show-harness]]의 VLM 직접 제어 경로와 대비하여, 코드 생성 제어 경로의 고유 안전 병목을 특정하며 코드-하네스 패러다임([[code-as-agent-harness]])의 평가 범위를 조작 성공률에서 안전 제약 준수로 확장한다.

## 🔗 관련 논문

- Show-Harness: Just a VLM Agent Can Play Robots
- In-Context Robot Learning with VLM Agents
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the S
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En

## 🏷️ 엔티티

- [[entities/obstacle-aware-harness.md|obstacle-aware-harness]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/goal-safety-signal-asymmetry.md|goal-safety-signal-asymmetry]]
- [[entities/planning-without-physical-constraint-encoding.md|planning-without-physical-constraint-encoding]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/safety-constraint-context-legibility.md|safety-constraint-context-legibility]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/show-harness.md|show-harness]]

## 📐 개념

- [[concepts/obstacle-aware-harness.md|obstacle-aware-harness]]
- [[concepts/goal-safety-signal-asymmetry.md|goal-safety-signal-asymmetry]]
- [[concepts/safety-constraint-context-legibility.md|safety-constraint-context-legibility]]
- [[concepts/structural-safety-enforcement.md|structural-safety-enforcement]]
- [[concepts/capability-safety-inseparability.md|capability-safety-inseparability]]

---
_LLM 분석으로 생성됨_
