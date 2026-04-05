# VideoSeek: Long-Horizon Video Agent with Tool-Guided Seeking

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-24  
**링크**: None

## 핵심 요약

**VideoSeek**는 긴 영상을 이해할 때 모든 프레임을 밀집 샘플링하는 기존 방식 대신, **비디오 논리 흐름(logic flow)을 활용해 정답에 필요한 핵심 증거만 능동적으로 탐색**하는 에이전트 프레임워크입니다. Think-Act-Observe 루프와 다중 granularity 관찰 도구를 결합하여, 기반 모델(GPT-5) 대비 **프레임 사용량을 93% 줄이면서도 LVBench에서 10.2점 향상**을 달성했습니다. CVPR 2026에 채택되었습니다.

## 인사이트

1. **영상 전체를 보지 않아도 된다** — 논리 흐름 기반의 선택적 탐색이 밀집 프레임 파싱보다 더 효과적이며 효율적이다.
2. **Think-Act-Observe 루프** 구조가 에이전트에게 질의 인식(query-aware) 탐색 능력을 부여하여, 필요한 시점의 정보만 점진적으로 수집할 수 있게 한다.
3. **다중 granularity 도구 설계**가 핵심으로, 영상을 거시적·미시적 수준에서 유연하게 관찰할 수 있어 다양한 질문 유형에 대응 가능하다.

## 응용 가능성

1. **장시간 영상 검색·감시 시스템** — 수시간 분량의 CCTV나 강의 영상에서 특정 이벤트를 저비용으로 빠르게 탐지하는 데 활용 가능하다.
2. **영상 기반 질의응답 서비스** — 영화·드라마·교육 콘텐츠에서 사용자 질문에 해당하는 장면을 효율적으로 찾아 답변하는 인터랙티브 에이전트에 적용 가능하다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-24.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-planning-over-mapf-agent-dependencies-via-multi-de.md]] (공통 Entity: LLM Agent)
