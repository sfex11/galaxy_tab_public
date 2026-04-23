# AgentFactory: A Self-Evolving Framework Through Executable Subagent Accumulation and Reuse

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.18000v1

## 💡 핵심 인사이트

에이전트의 성공 경험을 텍스트가 아닌 실행 가능한 서브에이전트 코드로 보존함으로써, 경험의 재현성과 재사용성을 근본적으로 향상시킨 자기 진화 패러다임이다.

## 📖 분석

## AgentFactory: 실행 가능한 서브에이전트 축적을 통한 자기 진화 프레임워크

**핵심 제안**: AgentFactory는 LLM 기반 에이전트의 자기 진화(self-evolution)에 새로운 패러다임을 제시한다. 기존 연구들이 성공 경험을 텍스트 프롬프트나 리플렉션으로 저장하는 데 그쳤다면, AgentFactory는 성공적인 태스크 솔루션을 **실행 가능한 서브에이전트 코드**로 보존한다. 이 서브에이전트들은 실행 피드백을 기반으로 지속적으로 개선되며, 축적·재사용된다.

**기존 접근과의 차별점**: 텍스트 기반 경험 저장은 복잡한 시나리오에서 효율적 재실행을 보장하지 못한다. AgentFactory는 경험을 코드로 결정화(crystallize)함으로써, 재현성과 실행 효율성을 동시에 확보한다. 이는 소프트웨어 엔지니어링의 모듈화 원칙을 에이전트 진화에 적용한 것으로 볼 수 있다.

**Wiki 연결점**:
- [[LLM Agent]]: AgentFactory는 LLM 에이전트의 자기 개선 메커니즘을 한 단계 발전시킨 연구로, 에이전트가 스스로 도구를 만들어 축적하는 구조를 제안한다.
- [[concepts/tool-use.md|tool use]]: 서브에이전트를 실행 가능한 코드로 저장·재사용하는 것은 도구 사용(tool-use)의 확장된 형태이며, 에이전트가 자신만의 도구 라이브러리를 자동 구축하는 셈이다.
- [[Multi-Agent System]]: 축적된 서브에이전트들이 협업하는 구조는 다중 에이전트 시스템의 동적 구성과 직결된다.
- Paper Circle(다중 에이전트 연구 논의 시스템)과 Gym-Anything(소프트웨어를 에이전트 환경으로 전환)는 AgentFactory의 서브에이전트 실행·평가 환경과 상보적 관계에 있다.

## 🔗 관련 논문

- 2026 04 09 gym anything turn any software into an agent envir
- 2026 04 09 paper circle an open source multi agent research d
- 2026 04 10 android coach improve online agentic training effi
- 2026 04 10 how much llm does a self revising agent actually n
- 2026 04 09 claw eval toward trustworthy evaluation of autonom

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/tool-use.md|tool-use]]
- [[concepts/multi-agent-system.md|multi-agent-system]]

---
_LLM 분석으로 재생성됨_
