# Affora: A Design System for Agent-Friendly Interfaces

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19125v1

## 💡 핵심 인사이트

에이전트-UI 호환성의 병목이 에이전트 측 능력이 아닌 인터페이스 측 가독성에 있을 때, 해법은 에이전트를 더 정교하게 만드는 것이 아니라 인간의 워크플로우를 보존하며 UI 자체를 인간과 기계의 이중 독자 설계로 전환하는 것이다.

## 📖 분석

# Affora: A Design System for Agent-Friendly Interfaces

**날짜**: 2026-09-18

## 요약

컴퓨터 사용 에이전트는 인간을 위해 설계된 소프트웨어를 조작하지만, 인간 중심 UI는 행동과 태스크 상태를 기계 독자에게 명확히 전달하지 못한다. Affora는 이를 후천적 접근성 계층(DOM 트리, 스크린샷 파싱)이 아닌 설계 시점 해법으로 푼다: 인간의 시각적 자유와 익숙한 워크플로우를 보존하면서 기계 독자용 행동·상태 단서를 컴포넌트에 내장한다. 세 개의 통제 실험(컴포넌트 구현, 시각 변이, 상호작용 설계 원칙)이 컴포넌트부터 완전한 사이트까지의 실증적 설계 지침을 도출한다.

## 기존 Wiki와의 관계

**문제 정의의 역전**: 기존 computer-use-agent 연구(JarvisGUI, CUA-Universe)는 에이전트가 인간용 UI에 적응하는 에이전트 측 해법이었다면, Affora는 배포 표면 자체를 에이전트의 일등 독자로 만드는 환경 측 해법으로 적응 부담의 방향을 뒤집는다.

**gui-grounding과의 상보성**: BAMI가 모호한 UI에 대한 그라운딩 편향을 에이전트 측에서 완화했다면, Affora는 인터페이스 설계 측에서 모호성을 원천 제거한다. 인간 독자용 시각 계약과 기계 독자용 명시 계약이 공존 가능함을 보여주는 이중 표현 계약 사례다.

**의의**: 에이전트-환경 공진화 논의가 훈련 환경(Environment Evolution, Terminal-Universe)에 머물렀다면, 본 논문은 생산 소프트웨어의 프런트엔드 설계 계층으로 이를 확장한다.

## 🔗 관련 논문

- BAMI: Training-Free Bias Mitigation in GUI Grounding
- JarvisGUI: Towards Cross-Device GUI Agents with Dynamic Task Composition
- CUA-Universe: A Scalable and Dynamic Environment for Hybrid GUI+CLI Agents
- Show-Harness: Just a VLM Agent Can Play Robots

## 🏷️ 엔티티

- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/gui-grounding.md|gui-grounding]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/machine-interpretable-interface-compliance.md|machine-interpretable-interface-compliance]]
- [[entities/interface-complexity-ambiguity.md|interface-complexity-ambiguity]]
- [[entities/design-probe.md|design-probe]]
- [[entities/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[entities/dual-readership-interface.md|dual-readership-interface]]

## 📐 개념

- [[concepts/dual-readership-interface.md|dual-readership-interface]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[concepts/machine-interpretable-interface-compliance.md|machine-interpretable-interface-compliance]]

---
_LLM 분석으로 생성됨_
