# BACE: LLM-based Code Generation through Bayesian Anchored Co-Evolution of Code and Test Populations

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-31  
**링크**: None

## 핵심 요약

BACE는 LLM 기반 코드 생성에서 생성된 테스트를 절대적 진리가 아닌 **불완전한 신호**로 모델링하는 베이지안 공진화 프레임워크이다. 기존 AgentCoder 등은 생성된 테스트를 그대로 신뢰하여 잘못된 코드가 결함 있는 테스트를 통과하거나, 올바른 코드가 잘못된 테스트에 맞춰 퇴화하는 문제가 있었다. BACE는 코드와 테스트 집단에 대한 **신뢰 분포(belief distribution)**를 유지하며 상호 증거에 기반해 베이지안 업데이트를 수행한다. 최소한의 공개 테스트 케이스를 앵커로 활용하여 자기검증 드리프트를 방지하며, LiveCodeBench v6에서 상용 및 오픈 소스 소형 모델 모두에서 우수한 성능을 달성했다.

## 인사이트

1. **생성된 테스트는 진리가 아니다** — 테스트를 확률적 노이즈 센서로 모델링함으로써 잘못된 테스트에 의한 코드 퇴화 문제를 근본적으로 해결했다.
2. **앵커링이 핵심이다** — 최소한의 공개 예제(public test cases)를 앵커로 활용하여, 코드와 테스트가 서로만 검증하며 함께 잘못된 방향으로 수렴하는 공진화 드리프트를 방지한다.
3. **범용성 확보** — 상용 LLM뿐 아니라 오픈 소스 소형 언어 모델에도 적용 가능하여, 실용적 활용 범위가 넓다.

## 응용 가능성

1. **자동화된 소프트웨어 개발 파이프라인** — CI/CD 환경에서 코드 생성과 테스트 생성을 동시에 수행하면서도 품질을 자체 검증할 수 있는 신뢰성 높은 에이전트 시스템 구축에 활용할 수 있다.
2. **코딩 교육 및 경진대회 보조 도구** — 경쟁 프로그래밍(LiveCodeBench 등) 문제 풀이에서 솔루션 후보를 자동 생성·검증하여, 학습자나 참가자의 문제 해결을 지원하는 도구로 응용 가능하다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-31-BACELLM-basedCodeGenerationthr.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-universal-yoco-for-efficient-depth-scaling.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-march-multi-agent-reinforced-self-check-for-llm-ha.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-02-extending-mona-in-camera-dropbox-reproduction-lear.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
