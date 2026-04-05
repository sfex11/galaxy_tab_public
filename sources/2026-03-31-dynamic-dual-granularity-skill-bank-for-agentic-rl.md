# Dynamic Dual-Granularity Skill Bank for Agentic RL

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-31  
**링크**: None

## 핵심 요약

D2Skill은 에이전트 강화학습(RL)에서 재사용 가능한 경험을 **이중 세분화(dual-granularity) 스킬 뱅크**로 조직화하는 프레임워크이다. **태스크 스킬**(고수준 가이던스)과 **스텝 스킬**(세밀한 의사결정 및 오류 수정)의 두 계층으로 경험을 저장하며, 동일 정책 하에서 기본 롤아웃과 스킬 주입 롤아웃을 쌍으로 실행하여 성능 차이를 힌사이트 유틸리티 신호로 활용한다. 이 신호로 스킬 뱅크 갱신과 정책 최적화를 동시에 수행하며, 리플렉션 기반 확장과 유틸리티 기반 가지치기로 스킬 뱅크를 동적으로 관리한다. ALFWorld·WebShop에서 성공률을 10~20%p 향상시켰다.

## 인사이트

1. **이중 세분화 설계**: 태스크 수준(전략)과 스텝 수준(전술)으로 스킬을 분리함으로써, 고수준 계획과 저수준 오류 복구를 동시에 지원할 수 있다.
2. **힌사이트 유틸리티 신호**: 스킬 유무에 따른 쌍대 롤아웃의 성능 차이를 학습 신호로 활용하여, 어떤 스킬이 실제로 유용한지를 사후적으로 판단하는 원칙적 메커니즘을 제공한다.
3. **동적 스킬 관리**: 리플렉션을 통한 스킬 확장과 유틸리티 기반 가지치기를 결합하여, 스킬 뱅크가 학습 과정에서 지속적으로 진화하며 불필요한 스킬이 자연스럽게 제거된다.

## 응용 가능성

1. **웹/GUI 에이전트 자동화**: 웹쇼핑·정보 검색 등 다단계 웹 상호작용 에이전트에 스킬 뱅크를 적용하여, 반복 태스크의 성공률과 효율성을 크게 높일 수 있다.
2. **LLM 기반 자율 에이전트의 지속 학습**: 대규모 언어모델 에이전트가 새로운 환경에서 경험을 축적·재활용하는 장기 메모리 시스템으로 확장하여, 도메인 전이 시에도 학습된 스킬을 활용할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

- Reinforcement Learning

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-31-DynamicDual-GranularitySkillBa.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-01-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-march-multi-agent-reinforced-self-check-for-llm-ha.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-multi-agent-video-recommenders-evolution-patterns-.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: LLM Agent)
