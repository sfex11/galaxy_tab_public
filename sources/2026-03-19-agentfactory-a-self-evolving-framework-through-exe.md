# AgentFactory: A Self-Evolving Framework Through Executable Subagent Accumulation and Reuse

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.18000v1

## 💡 핵심 인사이트

에이전트의 성공 경험을 텍스트가 아닌 실행 가능한 서브에이전트 코드로 보존함으로써, 자기 진화의 재현성과 효율성을 동시에 확보하는 새로운 패러다임을 제시한다.

## 📖 분석

## AgentFactory: 실행 가능한 서브에이전트 축적과 재사용을 통한 자기 진화 프레임워크

**핵심 아이디어**: 기존 LLM 에이전트 자기 진화 연구들이 성공 경험을 텍스트 프롬프트나 리플렉션으로 저장하는 데 그쳤다면, AgentFactory는 성공한 태스크 솔루션을 **실행 가능한 서브에이전트 코드**로 보존하는 새로운 패러다임을 제안한다. 이 서브에이전트들은 실행 피드백을 기반으로 지속적으로 정제되며, 축적·재사용된다.

**기존 접근과의 차별점**: 텍스트 기반 경험 저장은 복잡한 시나리오에서 효율적인 태스크 재실행을 안정적으로 보장하지 못한다. AgentFactory는 경험을 코드로 구체화함으로써 재현성과 실행 효율성을 동시에 확보한다. 이는 프롬프트 엔지니어링의 한계를 코드 생성으로 극복하려는 시도로 볼 수 있다.

**멀티 에이전트 시스템과의 관계**: 서브에이전트를 동적으로 생성·축적·재사용하는 구조는 멀티 에이전트 시스템의 확장으로 이해할 수 있다. 고정된 에이전트 구성이 아닌, 태스크에 따라 진화하는 에이전트 풀을 운용한다는 점에서 기존 MAS 연구를 한 단계 발전시킨다.

**LLM 에이전트 자기 진화의 새 방향**: 텍스트 경험 → 실행 가능 코드로의 전환은 에이전트의 학습 결과물이 더 구조화되고 검증 가능해짐을 의미한다. 강화학습에서의 정책 저장과 유사한 철학을 코드 수준에서 구현한 것으로 볼 수 있다.

## 🔗 관련 논문

- 2026 04 09 paper circle an open source multi agent research d
- 2026 04 09 gym anything turn any software into an agent envir
- 2026 04 10 android coach improve online agentic training effi
- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
