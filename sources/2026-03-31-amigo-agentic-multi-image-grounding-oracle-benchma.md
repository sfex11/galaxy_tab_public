# AMIGO: Agentic Multi-Image Grounding Oracle Benchmark

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-31  
**링크**: None

## 핵심 요약

AMIGO는 에이전틱 비전-언어 모델(VLM)의 **다중 이미지, 다중 턴 추론 능력**을 평가하는 벤치마크이다. 기존 평가가 단일 이미지·단일 턴에 집중하는 한계를 극복하기 위해, 시각적으로 유사한 이미지 갤러리에서 오라클이 비공개로 선택한 타겟 이미지를 모델이 Yes/No/Unsure 질문을 순차적으로 던져 식별하는 과제를 설계했다. 불확실성 하의 질문 선택, 다중 턴에 걸친 제약 추적, 증거 축적에 따른 세밀한 판별이라는 세 가지 핵심 역량을 평가하며, 오라클의 의도적 오류(노이즈)를 도입해 모델의 검증 행동과 강건성까지 측정한다.

## 인사이트

1. **기존 VLM 평가의 맹점 지적**: 단일 이미지·단일 턴 정답 맞추기 위주의 평가로는 실제 에이전트 환경에서 요구되는 장기적 추론·대화 능력을 측정할 수 없다.
2. **노이즈 내성 평가의 도입**: 오라클이 일관되지 않은 피드백(Unsure, 오답)을 줄 수 있는 설정을 통해, 모델이 불완전한 정보 속에서도 자기 검증하며 올바른 판단에 도달하는 능력을 측정한다.
3. **프로토콜 준수와 효율성의 동시 평가**: 단순 정답률뿐 아니라 질문 효율성, 프로토콜 위반(페널티 부과), 궤적 수준 진단 등 다차원 메트릭으로 에이전트의 행동 품질을 종합적으로 분석한다.

## 응용 가능성

1. **대화형 이미지 검색/추천 시스템**: 사용자가 원하는 상품(의류, 부동산 등)을 순차적 질문으로 좁혀가는 에이전트의 설계 및 성능 검증에 직접 활용할 수 있다.
2. **의료·보안 등 고위험 시각 판별 과제**: 시각적으로 유사한 대상(병변, 인물 등)을 불확실한 정보 속에서 정밀하게 식별해야 하는 분야의 AI 에이전트 신뢰성 평가 프레임워크로 확장 가능하다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-31-AMIGOAgenticMulti-ImageGroundi.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-textttyc-bench-benchmarking-ai-agents-for-long-ter.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-universal-yoco-for-efficient-depth-scaling.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
