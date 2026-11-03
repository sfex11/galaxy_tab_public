# FedReady: Bounded Agents for Federation Formation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03586v1

## 💡 핵심 인사이트

연합학습의 미해결 병목은 알고리즘이 아닌 반복되는 연합 구성(준비)이며, 원시 데이터 접근이 구조적으로 차단된 조건에서도 제한된 LLM 에이전트가 이 준비를 자동화할 수 있다.

## 📖 분석

# FedReady: Bounded Agents for Federation Formation (2026-11-04)

연합학습(FL) 런타임이 집계와 배포를 표준화한 뒤에도 남는 병목은 연합 구성(federation formation)이다 — 태스크 적합 사이트 선정, 로컬 데이터와 태스크 코드의 준비. 이 준비는 타겟이 바뀔 때마다 반복되며, 원시 기록과 사이트별 프라이빗 매핑은 교차 사이트 메시지에서 배제되어 수동 작업으로 남아 있었다.

## 핵심 기여

FedReady는 정보 접근이 제한된(bounded) LLM 에이전트들로 이 준비를 자동화한다. 에이전트가 공유 계약을 제안하고 사이트·데이터·코드 준비를 수행하되, 민감 정보 배제 제약을 준수하는 구조로 작동한다.

## 기존 Wiki와의 관계

- [[federated-learning]]: 기존 논의가 훈련 중 문제(연속학습·DP 예산)에 집중했다면, 본 논문은 학습 이전 준비 단계가 표준화 공백임을 진단한다.
- [[structural-isolation]]: 메시지 수준 정보 배제는 DP와 대비되는 구조적 격리로, 에이전트 자동화가 그 안에서 성립함을 보여준다.
- [[infrastructure-function-as-agent-action]]: 수동 준비 작업의 에이전트 액션 격상 사례. [[roboarchitect]](하네스 설계 자동화)·Gym-Anything(환경 저작)과 함께 '에이전트 = 인프라 준비자' 패턴의 FL 도메인 착지점.
- [[data-sovereignty]]: 데이터가 사이트에 머무는 전제 하의 교차 사이트 자동화 방법을 제시한다.
- [[scientific-workflow-agent]]: 다기관 연구의 물리적 전제 구축을 워크플로우 자동화 대상에 편입한다.

## 인사이트

인프라 표준화가 완료된 영역에서 남는 병목은 '준비'이며, 반복성 + 정보 제약이라는 조건이 정확히 제한된 에이전트 자동화의 적역이다.

## 🔗 관련 논문

- Collaborative AI agents for autonomous experimental research with soli
- Component-Aware Differential Privacy for Federated Multilingual Speech
- RoboArchitect: Automating the Design of Robotic Agents with Persistent
- Gym-Anything for Robotics: Scaling physical simulations with digital a

## 🏷️ 엔티티

- [[entities/federation-formation.md|federation-formation]]
- [[entities/federated-learning.md|federated-learning]]
- [[entities/data-sovereignty.md|data-sovereignty]]
- [[entities/federated-continual-learning.md|federated-continual-learning]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/zero-trust-agent-architecture.md|zero-trust-agent-architecture]]
- [[entities/data-exfiltration-prevention.md|data-exfiltration-prevention]]

## 📐 개념

- [[concepts/infrastructure-function-as-agent-action.md|infrastructure-function-as-agent-action]]
- [[concepts/structural-isolation.md|structural-isolation]]
- [[concepts/harness-design-automation.md|harness-design-automation]]
- [[concepts/composition-time-task-contract.md|composition-time-task-contract]]

---
_LLM 분석으로 생성됨_
