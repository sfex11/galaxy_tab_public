# HippoCamp: Benchmarking Contextual Agents on Personal Computers

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-03  
**링크**: None

## 핵심 요약

HippoCamp은 개인 컴퓨터 환경에서 AI 에이전트의 멀티모달 파일 관리 능력을 평가하기 위한 새로운 벤치마크다. 42.4GB, 2,000개 이상의 다양한 형식 파일로 구성된 실제 규모의 파일 시스템을 구축하고, 581개의 QA 쌍과 46,100개의 구조화된 궤적 데이터를 제공한다. 최신 상용 모델도 사용자 프로파일링 정확도가 48.3%에 불과하며, 멀티모달 인식과 증거 기반 추론이 주요 병목으로 확인되었다.

## 인사이트

1. 기존 벤치마크가 웹 상호작용·도구 사용 등 범용 환경에 집중한 반면, HippoCamp은 **개인 사용자 맥락 이해**라는 실질적 과제를 최초로 체계적으로 평가한다.
2. 최첨단 멀티모달 LLM조차 대규모 개인 파일에서의 **교차 모달 추론과 장거리 검색**에서 크게 실패하며, 정확도가 절반에도 못 미친다.
3. 단계별 실패 진단(46.1K 궤적 분석)을 통해 **멀티모달 인식과 증거 근거 연결(evidence grounding)**이 핵심 병목임을 정량적으로 규명했다.

## 응용 가능성

1. 개인 파일을 맥락적으로 이해하고 검색·정리해주는 **차세대 AI 개인 비서** 개발의 성능 기준점 및 평가 프레임워크로 활용할 수 있다.
2. 멀티모달 에이전트의 **약점 진단 도구**로 사용하여, 모델의 교차 모달 추론 및 근거 기반 응답 능력을 체계적으로 개선하는 데 기여할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-04-03-HippoCampBenchmarkingContextua.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-31-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-mecha-nudges-for-machines.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md]] (공통 Entity: LLM Agent)
