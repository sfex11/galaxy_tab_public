# Avatar: Toward Autonomous End-to-End Orchestration of Scientific Workflows using LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10509v1

## 💡 핵심 인사이트

에이전틱 추론의 도입 위치는 모델 선택이 아니라 아키텍처 분해(액터)와 플러그형 정책 교체의 설계 문제이며, 어댑터 검증 액션 카탈로그가 자율성과 위험 경계를 단일 메커니즘으로 동시에 실현한다.

## 📖 분석

Avatar는 과학 워크플로우 관리 시스템(WMS)의 오케스트레이션을 고정된 수제 규칙에서 LLM 에이전트 기반 자율 방식으로 전환하되, '어디에 에이전틱 추론을 도입할 것인가'를 아키텍처 파라미터로 격상시킨다. 오케스트레이터·실행자·출처 감시자(provenance monitor)로 분해된 액터 구조에서 각 액터의 결정 정책을 규칙 기반/LLM 기반으로 플러그형 교체 가능하게 설계하고, 어댑터 검증 액션 카탈로그가 LLM 결정을 사전 검증된 행동 공간으로 구속해 위험을 경계짓는다.

이는 [[computation-unit-meta-selection]]이 연산 단위(SLM vs LLM) 수준에서 다룬 선택 문제를 워크플로우 액터 수준의 정책 선택으로 확장한다. 어댑터 검증 액션 카탈로그는 [[representation-contract]]의 계약 관점과 [[interpretive-vs-structural-enforcement]]의 이분법에 새로운 구현 축을 제공한다 — 해석적/구조적 강제의 선택이 정적 설계가 아닌 런타임 구성 변수가 된다.

출처 감시자를 일급 액터로 배치한 것은 [[auditability-as-scaling-requirement]]의 최초 아키텍처 수준 구현 사례다. 기존 [[scientific-workflow-agent]]가 '연구 질문→워크플로우 번역 자동화'였다면, Avatar는 '오케스트레이션 정책 자체의 자율화'로 스코프를 확장하며 [[autoresearch]]의 연구 실행 자동화에 시스템 인프라 계층의 좌표를 추가한다.

## 🔗 관련 논문

- From Research Question to Scientific Workflow: Leveraging Agentic AI f (2026-04-25)

## 🏷️ 엔티티

- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/auditability-as-scaling-requirement.md|auditability-as-scaling-requirement]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[entities/interpretive-vs-structural-enforcement.md|interpretive-vs-structural-enforcement]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]

## 📐 개념

- [[concepts/pluggable-decision-policy.md|pluggable-decision-policy]]
- [[concepts/adapter-validated-action-catalog.md|adapter-validated-action-catalog]]
- [[concepts/provenance-monitor-actor.md|provenance-monitor-actor]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-10-saescientist-bench-can-ai-agents-conduct-autonomou]]: 자율 과학 연구 자동화라는 공통 목표에서 SAEScientist-Bench가 에이전트의 연구 수행 능력을 평가한다면, Avatar는 과학 워크플로우의 자율 오케스트레이션을 실행 인프라로 구현한다.
- → [[sources/2026-09-11-ideaambig-benchmarking-implementation-critical-gap]]: 자율 연구 워크플로우 자동화를 공유하며, 명세의 충분성(IdeaAMBIG)이 자율 오케스트레이션(Avatar) 성공의 입력 품질 조건이 되는 아이디어-실행 인터페이스 문제를 연결한다.
