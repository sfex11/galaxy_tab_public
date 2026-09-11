# Procedural Graphs: Self-Evolving Execution Structures for LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09153v1

## 💡 핵심 인사이트

에이전트의 절차 지식을 누적 히스토리 속 암묵적 생성에서 명시적 그래프 구조로 외재화하고 실행 중 자기 진화시키면, 긴 궤적의 목표 상실과 도구 순서 위반이 구조적으로 방어되지만 진화한 구조 자체의 검증이 새로운 재귀적 과제가 된다.

## 📖 분석

## 핵심 주장

LLM 에이전트의 절차 지식(무엇을, 어떤 순서로, 어떤 조건에서 수행할지)은 누적 히스토리 위의 비구속 생성 속에 암묵적으로만 존재하며, 궤적이 길어지면 목표 추적 상실·도구 순서 위반·비생산적 반복으로 균열된다. 지식 그래프가 선언 지식을 구조화하듯, 본 논문의 절차 그래프(Procedural Graph)는 절차 지식을 명시적 그래프로 구조화하고 실행 중 스스로 진화시킨다.

## 기존 Wiki와의 관계

- [[constraint-guided-plan-execution]]: RunAgent가 고정 자연어 계획을 제약으로 강제했다면, 절차 그래프는 계획 자체를 실행 중 변이 가능한 대상으로 만들어 '고정 계획' 전제를 해소한다.
- [[process-control-architecture]]: Box Maze가 토큰 스트림 수준 강제였다면, 절차 그래프는 제어 객체를 계획 그래프로 이동시킨 상보적 경로다.
- [[algorithm-system-translation-gap]]: 절차 지식의 토큰 평탄화([[semantic-structure-flattening]])를 구조적 명시로 역전시키는 구현 사례다.
- [[knowledge-state-drift]]: 목표 상실을 기억 소실이 아닌 절차 지식의 암묵성 문제로 재진단하고, 목표 추적을 그래프 노드로 외재화한다.

## 새 인사이트

자기 진화의 단위가 소스 코드(MOSS)나 스킬(SkillOS)에서 **런타임 실행 구조**로 축소되어 종단 간 진화의 가장 미세한 입자가 되었다. 그러나 실행 구조가 진화하면 구조 검증 자체가 재귀 문제가 된다([[verification-infrastructure-recursive-modification]]) — 실패 궤적이 절차 그래프에 흡수되면 후속 실행이 오염된 절차를 상속한다. [[procedural-identity]]는 명시적·이식 가능한 운반체를 얻지만, 진화에 따라 동일 명세의 에이전트 간 절차 분기라는 새로운 위험을 함께 얻는다.

## 🔗 관련 논문

- RunAgent: Interpreting Natural-Language Plans with Constrain
- Box Maze: A Process-Control Architecture for Reliable LLM Re
- MOSS: Self-Evolution through Source-Level Rewriting in Auton
- SkillOS: Learning Skill Curation for Self-Evolving Agents
- ADEMA: A Knowledge-State Orchestration Architecture for Long
- Design Docs Are All You Need: An AI-native Machine-Learning 

## 🏷️ 엔티티

- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/process-control-architecture.md|process-control-architecture]]
- [[entities/constraint-guided-plan-execution.md|constraint-guided-plan-execution]]
- [[entities/harness-mutability.md|harness-mutability]]
- [[entities/endogenous-self-evolution.md|endogenous-self-evolution]]
- [[entities/knowledge-state-drift.md|knowledge-state-drift]]
- [[entities/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[entities/procedural-identity.md|procedural-identity]]

## 📐 개념

- [[concepts/procedural-graph.md|procedural-graph]]
- [[concepts/procedural-knowledge-explicitation.md|procedural-knowledge-explicitation]]
- [[concepts/runtime-structure-self-evolution.md|runtime-structure-self-evolution]]
- [[concepts/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[concepts/semantic-structure-flattening.md|semantic-structure-flattening]]
- [[concepts/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[concepts/verification-infrastructure-recursive-modification.md|verification-infrastructure-recursive-modification]]
- [[concepts/execution-topology-invariance.md|execution-topology-invariance]]
- [[concepts/dynamic-lifecycle-safety.md|dynamic-lifecycle-safety]]
- [[concepts/code-as-agent-harness.md|code-as-agent-harness]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-11-convmem-convolutional-memory-for-long-context-reas]]: 둘 다 긴 궤적·컨텍스트에서의 목표 상실과 저하를 구조적으로 방어하려 하며, 절차 지식의 명시적 그래프화와 메모리의 합성곱 압축이라는 상보적 수단을 제안한다.
