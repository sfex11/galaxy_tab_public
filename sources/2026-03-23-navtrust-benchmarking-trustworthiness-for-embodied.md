# NavTrust: Benchmarking Trustworthiness for Embodied Navigation

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-23  
**링크**: None

## 핵심 요약

NavTrust는 체화된 내비게이션(VLN, OGN) 에이전트의 **신뢰성을 평가하는 최초의 통합 벤치마크**다. 기존 연구가 이상적 조건에서만 성능을 평가한 반면, NavTrust는 RGB, 깊이(Depth), 자연어 지시문 등 입력 모달리티에 현실적 손상(corruption)을 체계적으로 적용하여 성능 변화를 측정한다. 7개 최신 모델 평가 결과, 현실적 손상 조건에서 **상당한 성능 저하**가 확인되었으며, 4가지 완화 전략을 검증하고 실제 모바일 로봇에 배포하여 강건성 향상을 입증했다.

## 인사이트

1. 현재 최첨단 내비게이션 모델들은 이상적 환경에서는 우수하지만, 현실 세계의 센서 노이즈나 지시문 변형에 매우 취약하다.
2. RGB, 깊이, 언어 지시문 등 **다중 모달리티를 통합적으로 손상시키는 벤치마크**는 NavTrust가 최초이며, 이는 실제 배포 환경의 신뢰성 격차를 드러낸다.
3. 완화 전략 적용 후 실제 로봇에서 강건성 향상이 확인되어, **벤치마크 결과가 실환경에도 유효**함을 보여준다.

## 응용 가능성

1. **자율주행 로봇 및 서비스 로봇** 개발 시 센서 열화·환경 변화에 대한 내비게이션 시스템의 신뢰성 사전 검증 도구로 활용할 수 있다.
2. **VLN/OGN 모델의 학습 파이프라인**에 현실적 손상 데이터를 통합하여, 배포 전 강건성을 체계적으로 향상시키는 데 적용할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-23.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-26-code-review-agent-benchmark.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-03-textttyc-bench-benchmarking-ai-agents-for-long-ter.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-31-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
