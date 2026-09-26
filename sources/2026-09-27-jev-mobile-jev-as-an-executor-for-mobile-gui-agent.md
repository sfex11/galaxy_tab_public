# Jev-Mobile: Jev as an Executor for Mobile GUI Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30186v1

## 💡 핵심 인사이트

접근성 트리 같은 구조적 인터페이스 명세가 VLM 중심 에이전트 루프를 저빈도 계획-고빈도 실행으로 분해 가능하게 하며, 인터페이스 설계가 에이전트 아키텍처의 경제성을 결정하는 전제조건임을 입증한다.

## 📖 분석

Jev-Mobile은 모바일 GUI 에이전트의 지배적 패러다임 — 모든 상호작용 단계에서 VLM이 계획과 액션 그라운딩을 동시 수행 — 을 저빈도 VLM 계획과 고빈도 경량 실행으로 분해한다. VLM이 국소 목표를 지정하면 접근성 트리가 구조화된 실행 가능 액션 공간을 제공하고, 경량 실행기 Jev가 고빈도로 이를 수행하여 지연과 서빙 비용을 대폭 절감한다.

핵심 통찰은 인터페이스 구조가 아키텍처 경제성의 전제조건이라는 것이다. [[machine-interpretable-interface-compliance]] 관점에서, 접근성 트리라는 기계 판독 가능 명세 위에서는 그라운딩이 VLM의 시각 추론([[gui-grounding]])이 아닌 구조적 결정([[structured-action-grounding]])으로 대체 가능하다.

[[thought-action-separation]]이 안전 아키텍처로 제안되던 것과 달리 본 논문은 동일한 분리가 지연·비용 절감이라는 경제적 필연으로도 실현됨을 보여주며, 이는 [[computation-unit-meta-selection]]의 정적 아키텍처 버전이다. [[affora]]가 에이전트 친화적 인터페이스의 설계 방법을 제시했다면, 본 논문은 그 설계가 실제 아키텍처 비용 절감으로 이어지는 인과 경로를 모바일 도메인에서 완성한다.

## 🔗 관련 논문

- Affora: A Design System for Agent-Friendly Interfaces
- Semantic Action Graph: A Shared Representation for Agent Grounding
- Show-Harness: Just a VLM Agent Can Play Robots
- Cognitive Extensions for Dual-Process Language Agents: Memory and Self

## 🏷️ 엔티티

- [[entities/jev-mobile.md|jev-mobile]]

## 📐 개념

- [[concepts/lightweight-executor.md|lightweight-executor]]
- [[concepts/accessibility-tree-as-action-space.md|accessibility-tree-as-action-space]]
- [[concepts/low-frequency-planning-high-frequency-execution.md|low-frequency-planning-high-frequency-execution]]
- [[concepts/structured-action-grounding.md|structured-action-grounding]]
- [[concepts/interaction-frequency-asymmetry.md|interaction-frequency-asymmetry]]
- [[concepts/machine-interpretable-interface-compliance.md|machine-interpretable-interface-compliance]]
- [[concepts/thought-action-separation.md|thought-action-separation]]
- [[concepts/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[concepts/gui-grounding.md|gui-grounding]]
- [[concepts/dual-process-agent.md|dual-process-agent]]

---
_LLM 분석으로 생성됨_
