# SpecEyes: Accelerating Agentic Multimodal LLMs via Speculative Perception and Planning

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-26  
**링크**: None

## 핵심 요약

**SpecEyes**는 에이전틱 멀티모달 LLM(예: OpenAI o3, Gemini)의 순차적 실행 병목(인식→추론→도구호출 루프)을 해결하는 투기적(speculative) 가속 프레임워크입니다. 경량 MLLM이 투기적 플래너로서 실행 경로를 미리 예측하고, 신뢰도 기반 게이팅으로 불필요한 도구 호출을 조기 종료하며, 이기종 병렬 퍼널 구조로 처리량을 극대화합니다. 결과적으로 정확도를 유지하거나 최대 +6.7% 향상시키면서 **1.1~3.35배 속도 향상**을 달성했습니다.

## 인사이트

1. **에이전틱 깊이(agentic depth)** 라는 순차적 도구 호출 오버헤드가 멀티모달 에이전트의 핵심 병목이며, 이를 투기적 실행으로 깨뜨릴 수 있다.
2. 레이블 없는 **답변 분리성(answer separability) 기반 게이팅**으로 모델 스스로 신뢰도를 판단해 비싼 도구 체인을 조기 종료할 수 있다.
3. 경량 모델의 무상태(stateless) 동시성을 활용해 대형 모델의 직렬 실행을 가리는 **이기종 병렬 퍼널** 설계가 시스템 처리량을 크게 높인다.

## 응용 가능성

1. **실시간 시각 에이전트 서비스** — 자율주행, 로봇 비전 등 저지연이 필수인 멀티모달 에이전트 시스템에 적용하여 응답 속도를 대폭 개선할 수 있다.
2. **대규모 멀티모달 API 서빙** — 클라우드 환경에서 동시 요청 처리 시 병렬 퍼널 구조를 도입해 GPU 활용률과 처리량(throughput)을 극대화할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-26-SpecEyesAcceleratingAgenticMul.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-24-videoseek-long-horizon-video-agent-with-tool-guide.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-26-planning-over-mapf-agent-dependencies-via-multi-de.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
