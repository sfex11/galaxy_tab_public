# Agensh: Scaling Organizational Intelligence to 1,024 Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26781v1

## 💡 핵심 인사이트

다중 에이전트 시스템의 확장 상한은 개별 에이전트 능력이 아니라 중앙 오케스트레이터의 조정 용량이며, 조정을 집단 내부의 자기조직화 협력 루프로 이전하면 1,024 에이전트까지 확장 가능하다.

## 📖 분석

Agensh는 중앙 오케스트레이터 없이 자기조직화 협력 루프만으로 1,024 에이전트까지 확장하는 다중 에이전트 하네스다. 기존 하네스([[harness-scaling-axis]])의 확장이 중앙 오케스트레이터의 태스크 할당·워커 조율 용량에 의해 제한된다는 진단을 내리고, 이 병목을 구조적으로 제거한다.

이는 [[multi-agent-system]] 연구에 두 가지 기여를 한다. 첫째, [[stellar-colosseum]] 같은 many-agent 하네스와 달리 조정이 에이전트 집단 내부의 협력 루프에서 창발하므로, [[copying-collective-behavior]]와 [[communication-free-coordination]]이 야생·물리 시스템에서 관찰한 자기조직 패턴이 하네스 설계 원리로 채택된 사례다. 둘째, [[emergent-cheating-whistleblowing-swarm]]이 100 에이전트 규모에서 관찰한 창발적 사회 현상의 연구 인프라를 10배 규모로 확장하여, [[collective-vulnerability-propagation]]과 [[capability-cooperation-paradox]]의 스케일 의존성을 검증할 환경을 제공한다.

[[social-level-harness]] 관점에서 Agensh는 1,024 에이전트라는 규모에서 조정·감사·종료([[termination-guarantee-problem]])가 사회 수준 설계 대상임을 실증한다. 오케스트레이터 제거는 [[orchestration-transparency-illusion]]의 구조적 원천도 함께 제거하지만, 자기조직화의 통제 가능성이라는 새 질문을 연다.

## 🔗 관련 논문

- Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in Mathematics
- A Case Study on Emergent Cheating and Whistleblowing in Autonomous Research
- Copying explains the collective behavior of AI agents in the wild
- Recursive Multi-Agent Systems
- From Soliloquy to Agora: Memory-Enhanced LLM Agents with Decentralized Debate

## 🏷️ 엔티티

- [[entities/multi-agent-system.md|multi-agent-system]]
- [[entities/agent-coordination.md|agent-coordination]]
- [[entities/harness-scaling-axis.md|harness-scaling-axis]]
- [[entities/social-level-harness.md|social-level-harness]]
- [[entities/emergent-cheating-whistleblowing-swarm.md|emergent-cheating-whistleblowing-swarm]]
- [[entities/termination-guarantee-problem.md|termination-guarantee-problem]]

## 📐 개념

- [[concepts/orchestrator-bottleneck.md|orchestrator-bottleneck]]
- [[concepts/self-organized-cooperation-loop.md|self-organized-cooperation-loop]]
- [[concepts/organizational-intelligence.md|organizational-intelligence]]
- [[concepts/communication-free-coordination.md|communication-free-coordination]]
- [[concepts/collective-vulnerability-propagation.md|collective-vulnerability-propagation]]
- [[concepts/orchestration-transparency-illusion.md|orchestration-transparency-illusion]]
- [[concepts/interaction-tax.md|interaction-tax]]

---
_LLM 분석으로 생성됨_
