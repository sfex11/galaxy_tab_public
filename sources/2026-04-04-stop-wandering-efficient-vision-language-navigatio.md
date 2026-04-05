# Stop Wandering: Efficient Vision-Language Navigation via Metacognitive Reasoning

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-04  
**링크**: None

## 핵심 요약

**MetaNav**는 학습 없이(training-free) 동작하는 Vision-Language Navigation(VLN) 에이전트의 비효율적 탐색 문제(제자리 맴돌기, 중복 방문)를 해결하기 위해 **메타인지(metacognition)** 능력을 도입한 프레임워크이다. 3D 공간 메모리, 방문 이력 기반 계획, 그리고 탐색 정체 감지 시 LLM을 활용한 반성적 자기 교정의 세 가지 모듈로 구성된다. GOAT-Bench, HM3D-OVON, A-EQA 세 벤치마크에서 SOTA 성능을 달성하면서도 VLM 호출을 20.7% 줄여 효율성과 정확성을 동시에 향상시켰다.

## 인사이트

1. 기존 VLN 에이전트의 핵심 한계는 탐욕적(greedy) 프론티어 선택과 수동적 공간 기억에서 비롯되며, 이는 자기 모니터링 능력의 부재로 귀결된다.
2. 에이전트가 "정체 상태"를 스스로 감지하고 LLM을 통해 교정 규칙을 생성하는 반성적 메커니즘이 탐색 효율을 획기적으로 개선한다.
3. 방문 이력에 페널티를 부여하는 단순한 전략만으로도 중복 방문을 크게 줄일 수 있으며, 이를 메타인지와 결합하면 시너지 효과가 발생한다.

## 응용 가능성

1. **가정용 로봇/자율주행**: 실내 환경에서 자연어 명령을 따르는 서비스 로봇이나 배달 로봇에 적용하여, 비효율적 경로 탐색 없이 목적지에 도달하는 데 활용할 수 있다.
2. **게임/메타버스 AI NPC**: 3D 가상 환경에서 사용자의 자연어 지시를 이해하고 자기 교정하며 효율적으로 탐색하는 지능형 NPC 개발에 응용할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-04-StopWanderingEfficientVision-L.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-05-actionparty-multi-subject-action-binding-in-genera.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-planning-over-mapf-agent-dependencies-via-multi-de.md]] (공통 Entity: LLM Agent)
