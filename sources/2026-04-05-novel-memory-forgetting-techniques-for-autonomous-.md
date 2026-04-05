# Novel Memory Forgetting Techniques for Autonomous AI Agents: Balancing Relevance and Efficiency

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-05  
**링크**: None

## 핵심 요약

자율 AI 에이전트의 장기 대화에서 메모리가 무한히 축적되면 시간적 성능 저하와 허위 기억(false memory) 전파가 발생한다. 본 논문은 **적응적 예산 기반 망각 프레임워크(Adaptive Budgeted Forgetting Framework)**를 제안하며, **최신성(Recency)**, **빈도(Frequency)**, **의미적 정렬(Semantic Alignment)** 세 가지 차원의 점수를 결합하여 관련성이 낮은 기억을 전략적으로 제거한다. LOCOMO, LOCCO, MultiWOZ 벤치마크에서 F1 점수가 기존 0.583 기준선을 초과하고, 허위 기억률(6.8%)을 줄이면서도 컨텍스트 윈도우를 확장하지 않고 추론 성능을 유지하는 결과를 보였다.

## 인사이트

1. 메모리를 무조건 유지하는 것이 아니라 **전략적으로 망각하는 것**이 장기 대화 에이전트의 성능을 오히려 향상시킨다.
2. 최신성·빈도·의미적 관련성을 결합한 **다차원 점수 체계**가 단일 기준 방식보다 어떤 기억을 버릴지 더 정교하게 판단할 수 있다.
3. 제한된 컨텍스트 윈도우 안에서 **유한 예산 최적화(bounded optimization)**를 적용하면, 윈도우 크기를 늘리지 않고도 추론 품질을 유지할 수 있다.

## 응용 가능성

1. **장기 고객 상담 챗봇** — 수백 턴 이상의 대화에서 오래된 무관한 정보를 자동 정리하여 응답 정확도와 일관성을 높일 수 있다.
2. **자율 AI 에이전트(코딩 에이전트, 업무 자동화 등)** — 장시간 작업 수행 시 컨텍스트 오염 없이 핵심 정보만 유지하여 효율적인 의사결정을 지속할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-05-NovelMemoryForgettingTechnique.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-claudini-autoresearch-discovers-state-of-the-art-a.md]] (공통 Entity: LLM Agent)
