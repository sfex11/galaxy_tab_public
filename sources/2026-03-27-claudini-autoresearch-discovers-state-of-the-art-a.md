# Claudini: Autoresearch Discovers State-of-the-Art Adversarial Attack Algorithms for LLMs

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-27  
**링크**: None

## 핵심 요약

Claudini는 Claude Code 기반 자율연구(autoresearch) 파이프라인을 통해 LLM에 대한 새로운 화이트박스 적대적 공격 알고리즘을 자동으로 발견하는 연구다. 기존 GCG 등의 공격 구현을 출발점으로 반복적으로 개선하여, 기존 30개 이상의 방법을 크게 능가하는 공격 알고리즘을 발견했다. GPT-OSS-Safeguard-20B 대상 CBRN 쿼리에서 기존 방법의 ASR(공격 성공률) ≤10% 대비 최대 40%를 달성했고, 서로게이트 모델에서 최적화한 공격이 Meta-SecAlign-70B에 전이되어 100% ASR(기존 최고 56%)을 기록했다.

## 인사이트

1. **자동화 적합성**: 화이트박스 적대적 공격은 기존 구현이라는 강력한 출발점과 정량적 피드백(최적화 목표)이 존재하여 LLM 에이전트 기반 자동 연구에 특히 적합한 영역이다.
2. **전이 공격력**: 서로게이트 모델에서 발견된 공격이 미공개 모델에도 효과적으로 전이되어, 실제 방어 체계 평가에 활용할 수 있는 범용성을 보여준다.
3. **점진적 연구 자동화**: 이 연구는 LLM 에이전트가 단순 코드 작성을 넘어 점진적인 AI 안전·보안 연구 자체를 자동화할 수 있음을 실증한 초기 사례다.

## 응용 가능성

1. **AI 안전 레드팀 자동화**: 모델 배포 전 자동화된 적대적 공격 탐색 파이프라인을 구축하여, 안전성 취약점을 사전에 체계적으로 발견하고 방어를 강화할 수 있다.
2. **범용 자율연구 프레임워크**: 정량적 피드백이 가능한 다른 연구 영역(프롬프트 최적화, 모델 정렬 등)에도 동일한 autoresearch 파이프라인을 확장 적용할 수 있다.

## 추출된 엔티티

- LLM Agent
- Claude 3.5

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-27-ClaudiniAutoresearchDiscoversS.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-03-26-code-review-agent-benchmark.md]] (공통 Entity: Claude 3.5, LLM Agent)
- [[sources/2026-04-03-textttyc-bench-benchmarking-ai-agents-for-long-ter.md]] (공통 Entity: Claude 3.5, LLM Agent)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-02-reward-based-online-llm-routing-via-neuralucb.md]] (공통 Entity: Claude 3.5)
- [[sources/2026-04-02-architecting-secure-ai-agents-perspectives-on-syst.md]] (공통 Entity: LLM Agent)
