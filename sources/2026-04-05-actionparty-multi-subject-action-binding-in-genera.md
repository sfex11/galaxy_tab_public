# ActionParty: Multi-Subject Action Binding in Generative Video Games

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-05  
**링크**: None

## 핵심 요약

ActionParty는 비디오 디퓨전 모델에서 **다중 에이전트의 액션 바인딩 문제**를 해결한 연구입니다. 기존 비디오 월드 모델은 단일 에이전트만 제어할 수 있었으나, ActionParty는 **Subject State Tokens**(각 주체의 상태를 지속적으로 포착하는 잠재 변수), **공간 바이어싱을 활용한 공동 모델링 아키텍처**, 그리고 **분리된 제어(Disentangled Control)** 메커니즘을 통해 특정 행동을 해당 주체에 정확히 연결합니다. 이를 통해 최대 7명의 플레이어를 동시에 제어할 수 있으며, Melting Pot 벤치마크의 46개 환경에서 액션 추종 정확도와 주체 일관성 향상을 입증했습니다.

## 인사이트

1. 기존 비디오 디퓨전 모델의 근본적 한계는 "액션 바인딩" 문제, 즉 특정 행동을 특정 주체에 올바르게 연결하지 못하는 것이었다.
2. Subject State Tokens이라는 잠재 변수를 도입하여 각 주체의 상태를 프레임 간 지속적으로 추적함으로써 다중 에이전트 정체성 유지 문제를 해결했다.
3. 글로벌 프레임 렌더링과 개별 주체 업데이트를 공간적으로 분리하는 아키텍처 설계가 다중 제어의 핵심이다.

## 응용 가능성

1. **생성형 비디오 게임**: 다수의 플레이어가 동시에 참여하는 인터랙티브 게임 환경을 비디오 디퓨전으로 시뮬레이션할 수 있다.
2. **다중 에이전트 시뮬레이션**: 로보틱스, 자율주행 등에서 여러 에이전트가 상호작용하는 복잡한 시나리오를 생성·테스트하는 데 활용할 수 있다.

## 추출된 엔티티

- LLM Agent
- Multi-Agent System

## 추출된 개념

- Multi-Agent System
- World Model

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-05-ActionPartyMulti-SubjectAction.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-26-planning-over-mapf-agent-dependencies-via-multi-de.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-03-26-biased-error-attribution-in-multi-agent-human-ai-s.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-03-27-march-multi-agent-reinforced-self-check-for-llm-ha.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-03-multi-agent-video-recommenders-evolution-patterns-.md]] (공통 Entity: Multi-Agent System, LLM Agent)
