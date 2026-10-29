# TANDEM: Balancing Centralized and Decentralized Critics to Address the Information Gap in Complex Multi-Agent Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37592v1

## 💡 핵심 인사이트

CTDE 분산 정책의 실패는 능력 부족이 아니라 '전역 정보 조건에서 훈련되어 국소 정보 조건에서 실행되는' 정보 간극의 구조적 귀결이며, 중앙·분산 비평자의 균형으로 훈련 시점에 봉합할 수 있다.

## 📖 분석

# TANDEM: 중앙·분산 비평자 균형 (2026-10-29)

CTDE 협력적 MARL의 구조적 결함을 진단한다: 전역 상태를 관찰하는 중앙 비평자로 훈련된 분산 정책은 실행 시점에 가지지 못할 정보에 의존하도록 최적화된다. 이 **정보 간극(information gap)**은 부분 관측·관측 노이즈·개방성(에이전트·태스크 집합의 실행 중 변화)에서 확대된다. TANDEM은 중앙·분산 비평자의 균형 결합으로 훈련 시점에 간극을 봉합한다. 기존 Wiki의 TANDEM([[tandem-task-and-motion-planning-with-as-needed-dem]], TAMP 시연)과는 별개 논문임에 유의한다.

## Wiki 연결

- [[training-inference-mismatch]]가 엔진 간 수치 드리프트(TIM)였다면, 본 논문은 그 **정보 구조 버전** — 훈련·실행 간 정보 가용성 불일치 — 을 제공하여 불일치 분류를 수치·정보 양축으로 확장한다.
- [[critic-free-optimization]]([[bellman-policy-optimization]])이 가치 추정 회피 경로라면, TANDEM은 비평자를 유지하되 **정보 조건을 정합화**하는 제2 경로로, '전면 중앙 → 균형 하이브리드 → 회피' 해법 스펙트럼을 완성한다.
- [[local-coherence-global-incoherence]]의 생성 메커니즘을 설명한다: 전역 관측 하 최적화된 분산 정책의 국소 최적-집단 비합리성이 정보 간극의 직접 귀결이다.
- [[non-stationary-dynamics]]·[[team-formation-idiosyncrasy]]: 개방성이 간극을 확대한다는 발견으로, 팀 구성 변화의 비용이 실행 성능 차원에서 정량화된다.
- [[communication-free-coordination]]: 훈련은 통신 풍부(전역 상태), 실행은 통신 없음(국소 관측)의 비대칭이 조정 실패의 숨은 원인임을 규명한다.

## 🔗 관련 논문

- Multi-agent Scaling Across Disjunctive and Compensatory Tasks
- AgentWorld: Benchmarking Long-Horizon Collaboration of Multi-agent LLM

## 🏷️ 엔티티

- [[entities/tandem-critics.md|tandem-critics]]
- [[entities/multi-agent-reinforcement-learning.md|multi-agent-reinforcement-learning]]
- [[entities/critic-free-optimization.md|critic-free-optimization]]
- [[entities/seeq.md|seeq]]
- [[entities/hystar.md|hystar]]

## 📐 개념

- [[concepts/ctde-information-gap.md|ctde-information-gap]]
- [[concepts/training-inference-mismatch.md|training-inference-mismatch]]
- [[concepts/local-coherence-global-incoherence.md|local-coherence-global-incoherence]]
- [[concepts/non-stationary-dynamics.md|non-stationary-dynamics]]
- [[concepts/communication-free-coordination.md|communication-free-coordination]]
- [[concepts/state-value-estimation-avoidance.md|state-value-estimation-avoidance]]
- [[concepts/information-usability-gap.md|information-usability-gap]]
- [[concepts/imperfect-perception.md|imperfect-perception]]
- [[concepts/team-formation-idiosyncrasy.md|team-formation-idiosyncrasy]]
- [[concepts/dynamic-task-composition.md|dynamic-task-composition]]

---
_LLM 분석으로 생성됨_
