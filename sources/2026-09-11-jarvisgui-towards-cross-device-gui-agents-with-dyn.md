# JarvisGUI: Towards Cross-Device GUI Agents with Dynamic Task Composition

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10451v1

## 💡 핵심 인사이트

단일 기기·정적 태스크 벤치마크는 중간 결과 전달·공유 상태 유지·이종 환경 조율이라는 실세계 워크플로우의 핵심 차원을 평가하지 못해 에이전트 준비도를 구조적으로 과대평가한다.

## 📖 분석

# JarvisGUI: 크로스 디바이스 GUI 에이전트와 동적 태스크 구성

## 핵심 주장
실제 GUI 사용은 여러 기기·플랫폼에 걸친 워크플로우(중간 결과 전달, 공유 상태 유지, 이종 환경 조율)를 요구하지만, 기존 벤치마크는 단일 기기·정적 태스크만 평가하여 실세계 준비도를 과대평가한다.

## 기존 Wiki와의 관계
- **CUA-Universe와 상보적 축**: CUA-Universe가 GUI+CLI 이종 실행 모달리티로 실세계 복잡성을 확장했다면, 본 논문은 물리적·플랫폼적 이질성(크로스 디바이스)을 추가하여 단일 화면·단일 기기 벤치마크가 놓친 직교 차원을 형성한다.
- **[[benchmark-specification-gap]]의 GUI 발현**: 벤치마크가 명세하지 않은 차원(중간 결과 이전, 공유 상태)이 실제 워크플로우 성공을 결정한다.
- **[[evaluation-deployment-unit-mismatch]]**: 평가 단위(단일 기기·정적 태스크)와 배포 단위(다중 기기·동적 워크플로우)의 불일치가 '지나치게 낙관적인 준비도 평가'를 산출한다.

## 새 인사이트
1. **동적 태스크 구성**: 태스크를 사전 정의 항목이 아닌 실행 시점에 조립되는 구조로 재정의한다. 정적 벤치마크 패러다임 자체에 대한 재검토를 요구하며, Claw-Eval-Live의 실시간 신호 갱신 논리와 공명한다.
2. **공유 상태의 기기 간 확장**: PSI가 공유 상태를 AI 생성물 조율의 누락 계층으로 진단한 것을 GUI 에이전트로 확장한다. 기기 경계를 넘는 상태 유지·전달은 [[stateless-architecture-vulnerability]]와 유사한 취약점 축을 새로 연다.

## 연결점
[[computer-use-agent]]·[[gui-grounding]]의 평가 지형에 '기기 경계 번역 능력'이라는 새 검증 축을 추가하고, [[cross-platform-evolution]]·[[task-reality-divergence]]·[[sandbox-liveworld-gap]] 논의를 GUI 워크플로우 도메인으로 구체화한다. 새 엔티티 cross-device-workflow와 dynamic-task-composition의 원천 정의를 제공한다.

## 🔗 관련 논문

- CUA-Universe: A Scalable and Dynamic Environment for Hybrid GUI+CLI Agents
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows
- DV-World: Benchmarking Data Visualization Agents in Real-World Scenarios
- PSI: Shared State as the Missing Layer for Coherent AI-Generated Code

## 🏷️ 엔티티

- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/gui-grounding.md|gui-grounding]]
- [[entities/cross-platform-evolution.md|cross-platform-evolution]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[entities/shared-state-architecture.md|shared-state-architecture]]
- [[entities/task-reality-divergence.md|task-reality-divergence]]
- [[entities/cross-device-workflow.md|cross-device-workflow]]
- [[entities/dynamic-task-composition.md|dynamic-task-composition]]

## 📐 개념

- [[concepts/intermediate-result-transfer.md|intermediate-result-transfer]]
- [[concepts/evaluator-assumption.md|evaluator-assumption]]
- [[concepts/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[concepts/stateless-architecture-vulnerability.md|stateless-architecture-vulnerability]]
- [[concepts/device-heterogeneity-coordination.md|device-heterogeneity-coordination]]

---
_LLM 분석으로 생성됨_
