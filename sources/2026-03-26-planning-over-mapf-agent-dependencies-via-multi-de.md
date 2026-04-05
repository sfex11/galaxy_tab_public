# Planning over MAPF Agent Dependencies via Multi-Dependency PIBT

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-26  
**링크**: None

## 핵심 요약

**MD-PIBT(Multi-Dependency PIBT)**는 기존 PIBT 알고리즘의 한계를 극복한 다중 에이전트 경로 탐색(MAPF) 프레임워크입니다. 기존 PIBT는 최대 하나의 다른 에이전트와 충돌하는 경로만 탐색할 수 있었으나, MD-PIBT는 **에이전트 간 의존성(dependency)**을 기반으로 여러 에이전트의 상호작용을 동시에 고려하여 경로를 계획합니다. 특정 파라미터 설정으로 기존 PIBT와 EPIBT를 재현할 수 있으며, 그 이상의 새로운 계획 전략도 표현 가능합니다. 최대 10,000개의 에이전트, 다양한 운동학적 제약(pebble motion, rotation, differential drive) 환경에서 효과적으로 동작합니다.

## 인사이트

1. **규칙 기반에서 의존성 기반으로의 전환**: PIBT의 우선순위 상속 로직을 "에이전트 의존성"이라는 더 일반적인 개념으로 재정의하여 프레임워크의 표현력을 크게 확장했다.
2. **기존 알고리즘의 통합**: MD-PIBT는 PIBT와 EPIBT를 특수 사례(special case)로 포함하는 상위 프레임워크로, 기존에 표현 불가능했던 새로운 계획 전략까지 가능하게 한다.
3. **단일 의존성의 병목 해소**: 기존 PIBT가 한 번에 하나의 에이전트 충돌만 처리할 수 있던 제약을 다중 의존성으로 확장하여, 혼잡 환경에서의 계획 품질을 근본적으로 개선했다.

## 응용 가능성

1. **대규모 물류 창고 자동화**: 수천 대의 AGV(무인운반차)가 동시에 운영되는 아마존 스타일 풀필먼트 센터에서, 혼잡 구간의 교착 상태 없이 실시간 경로 계획에 활용할 수 있다.
2. **자율주행 로봇 군집 제어**: 차동 구동(differential drive) 등 실제 로봇의 운동학적 제약을 지원하므로, 공장·병원·배달 환경에서 다양한 크기와 형태의 로봇 군집 협조 주행에 적용 가능하다.

## 추출된 엔티티

- LLM Agent
- Multi-Agent System

## 추출된 개념

- Multi-Agent System

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-26-PlanningoverMAPFAgentDependenc.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-05-actionparty-multi-subject-action-binding-in-genera.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-02-the-triadic-cognitive-architecture-bounding-autono.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-03-31-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-03-multi-agent-video-recommenders-evolution-patterns-.md]] (공통 Entity: Multi-Agent System, LLM Agent)
