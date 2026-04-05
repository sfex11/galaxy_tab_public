# $\texttt{YC-Bench}$: Benchmarking AI Agents for Long-Term Planning and Consistent Execution

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-03  
**링크**: None

## 핵심 요약

**YC-Bench**는 LLM 에이전트의 장기 전략적 일관성을 평가하는 벤치마크로, 에이전트가 1년(수백 턴) 동안 가상 스타트업을 운영하며 직원 관리, 계약 선택, 수익성 유지를 수행한다. 초기 자본 $200K로 시작하여 적대적 클라이언트와 증가하는 인건비 속에서 의사결정해야 한다. 12개 모델 평가 결과, Claude Opus 4.6이 최종 자산 $127만으로 1위를 기록했고, 대부분의 모델은 초기 자본조차 유지하지 못했다. 스크래치패드 활용이 성공의 가장 강력한 예측 변수로 나타났다.

## 인사이트

1. **적대적 클라이언트 탐지 실패**가 파산의 47%를 차지하며, 현재 AI 에이전트의 기만 탐지 능력이 크게 부족함을 보여준다.
2. **스크래치패드(메모) 활용**이 성공의 핵심 예측 변수로, 제한된 컨텍스트 윈도우에서 정보 지속성을 유지하는 능력이 장기 계획의 핵심이다.
3. 초기 자본을 유지한 모델이 12개 중 3개뿐으로, **장기 전략적 일관성**은 현재 프론티어 모델에서도 여전히 미해결 과제이다.

## 응용 가능성

1. **AI 에이전트 신뢰성 평가**: 자율 에이전트를 실제 비즈니스 운영에 배치하기 전, 장기적 의사결정 능력과 적대적 상황 대응력을 사전 검증하는 프레임워크로 활용할 수 있다.
2. **에이전트 메모리 아키텍처 개선**: 스크래치패드가 성공의 핵심이라는 발견을 바탕으로, 외부 메모리 및 정보 지속성 메커니즘을 강화한 차세대 에이전트 설계에 적용할 수 있다.

## 추출된 엔티티

- LLM Agent
- Claude 3.5

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-03-textttYC-BenchBenchmarkingAIAg.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-26-code-review-agent-benchmark.md]] (공통 Entity: Claude 3.5, LLM Agent)
- [[sources/2026-03-27-claudini-autoresearch-discovers-state-of-the-art-a.md]] (공통 Entity: Claude 3.5, LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
