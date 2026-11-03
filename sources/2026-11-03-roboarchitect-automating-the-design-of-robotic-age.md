# RoboArchitect: Automating the Design of Robotic Agents with Persistent Memory

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42141v1

## 💡 핵심 인사이트

체화 에이전트의 새 환경 적응에서 1차 최적화 대상은 정책 가중치가 아니라 하네스 코드이며, 그 설계 주체는 인간에서 코딩 에이전트로 이동 가능하다.

## 📖 분석

# RoboArchitect: Automating the Design of Robotic Agents with Persistent Memory (2026-11-03)

동결된 로봇 정책의 성능이 그 위의 하네스(제어 코드)에 크게 좌우된다는 관찰 위에서, 로봇·벤치마크마다 수작업으로 재설계되던 하네스의 설계를 자동화하는 시스템. 코딩 모델이 롤아웃을 관찰하고 실패를 진단해 하네스 코드를 반복 개정하며, 영구 메모리에 설계 지식을 축적한다.

## Wiki에서의 위치

하네스 설계 주체의 인간→에이전트 전환([[harness-subject-internalization]])의 체화 도메인 실현이다. 동결 정책+자동 설계 하네스가 파인튜닝의 강력한 대안이라는 결과는 정책 가중치와 하네스가 분리 가능한 최적화 축임([[model-harness-decomposability]])을 실증하며, 하네스가 능력 번역자([[harness-as-capability-translator]])라면 번역 규칙 자체가 생성 가능한 대상임을 확정한다. 관찰→진단→개정 루프는 [[failure-guided-harness-growth]]의 로봇 버전이고, 실패는 하네스 개정의 인과 데이터([[failure-as-causal-data]])로 소비된다.

## 연결점

- [[show-harness]]·[[embodied-harness]]: 수작업 로봇 하네스 구축에 이은 설계 자동화 축
- [[robot-skill-as-code]]: 하네스 코드가 감사 가능한 로봇 능력 아티팩트로 영구 메모리에 축적
- [[validated-skill-library]]·[[skill-as-external-state]]: 설계 지식의 재사용 가능 외부 상태화
- [[coding-agent-domain-deboundarying]]: 코딩 에이전트가 로봇 에이전트 설계의 저자가 되는 경계 확장
- [[harness-task-matching-bottleneck]]: 로봇별 하네스 매칭 병목에 대한 자동 매칭 해법
- [[scale-conditional-training-strategy]]: 적응 수단 스펙트럼에 파인튜닝 대안 경로 추가

## 🔗 관련 논문

- Show-Harness: Just a VLM Agent Can Play Robots
- Learning Meta-Skills for Agent Harness Design in Test-Time AI4AI
- Harness Learning Enables Generalizable Test-Time Adaptation
- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation
- RAPID: Robot Agentic Programming from Demonstrations
- SwapBot: Tool-Centric Robot Manipulation via Interchangeable

## 🏷️ 엔티티

- [[entities/roboarchitect.md|roboarchitect]]
- [[entities/harness-engineering.md|harness-engineering]]
- [[entities/robot-skill-as-code.md|robot-skill-as-code]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/embodied-harness.md|embodied-harness]]
- [[entities/show-harness.md|show-harness]]
- [[entities/coding-agent-domain-deboundarying.md|coding-agent-domain-deboundarying]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]

## 📐 개념

- [[concepts/harness-subject-internalization.md|harness-subject-internalization]]
- [[concepts/harness-as-capability-translator.md|harness-as-capability-translator]]
- [[concepts/model-harness-decomposability.md|model-harness-decomposability]]
- [[concepts/failure-guided-harness-growth.md|failure-guided-harness-growth]]
- [[concepts/failure-as-causal-data.md|failure-as-causal-data]]
- [[concepts/harness-learning.md|harness-learning]]
- [[concepts/harness-task-matching-bottleneck.md|harness-task-matching-bottleneck]]
- [[concepts/harness-capability-boundary.md|harness-capability-boundary]]
- [[concepts/harness-as-nonparametric-policy-layer.md|harness-as-nonparametric-policy-layer]]
- [[concepts/scale-conditional-training-strategy.md|scale-conditional-training-strategy]]
- [[concepts/harness-design-automation.md|harness-design-automation]]

---
_LLM 분석으로 생성됨_
