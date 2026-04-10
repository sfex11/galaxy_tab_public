# PSI: Shared State as the Missing Layer for Coherent AI-Generated Instruments in Personal AI Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08529v1

## 💡 핵심 인사이트

AI가 생성한 개별 도구들의 고립 문제를 공유 상태 버스(shared personal-context bus)를 통해 해결하여, 독립 모듈들을 크로스 모듈 추론이 가능한 coherent instrument로 전환할 수 있다.

## 📖 분석

## PSI: Shared State as the Missing Layer for Coherent AI-Generated Instruments in Personal AI Agents

### 개요
PSI는 자연어 요청으로 생성된 개인용 AI 도구(모듈)들이 생성 후 서로 고립되는 문제를 해결하기 위한 **공유 상태(shared-state) 아키텍처**를 제안한다. 독립적으로 생성된 모듈들을 persistent하고 상호 연결된 'instrument'로 전환하며, GUI와 범용 채팅 에이전트 양쪽에서 접근 가능하게 만든다. 핵심 메커니즘은 각 모듈이 현재 상태와 write-back affordance를 **공유 personal-context bus**에 게시하여, 크로스 모듈 추론과 동기화된 액션을 가능케 하는 것이다.

### 기존 Wiki와의 관계
- **[[llm-agent]]**: PSI의 generic chat agent는 LLM 기반 에이전트가 도구들을 오케스트레이션하는 구조로, LLM Agent 패러다임의 확장이다. 특히 에이전트가 여러 도구의 상태를 읽고 쓸 수 있는 affordance 설계가 핵심이다.
- **[[tool-use]]**: 개별 도구 호출을 넘어, 도구 간 상태 공유와 조율이라는 새로운 차원의 tool-use 패턴을 제시한다.
- **[[multi-agent-system]]**: 다수의 AI 생성 모듈이 공유 버스를 통해 협업하는 구조는 멀티에이전트 시스템의 아키텍처적 변형으로 볼 수 있다.

### 주요 기여
1. 생성형 AI 도구의 **사후 통합(post-creation integration)** 문제를 최초로 체계적으로 다룸
2. Shared personal-context bus를 통한 **크로스 모듈 추론** 메커니즘 제안
3. Chat-complementary artifact 개념으로 GUI와 대화형 인터페이스의 통합 모델 제시

### 연결점
- [[sources/2026-04-08-filegram-grounding-agent-personalization-in-file-s|FileGram]]: 개인화된 에이전트의 파일 기반 그라운딩과 PSI의 개인 컨텍스트 버스는 상호보완적 접근
- [[sources/2026-04-09-gym-anything-turn-any-software-into-an-agent-envir|Gym-Anything]]: 소프트웨어를 에이전트 환경으로 전환하는 관점에서 PSI의 모듈-instrument 전환과 유사한 철학 공유

## 🔗 관련 논문

- 2026 04 08 filegram grounding agent personalization in file s
- 2026 04 09 gym anything turn any software into an agent envir
- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/tool-use.md|tool-use]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/shared-state-architecture.md|shared-state-architecture]]
- [[concepts/personal-ai-agent.md|personal-ai-agent]]
- [[concepts/context-bus.md|context-bus]]

---
_LLM 분석으로 생성됨_
