# MARCH: Multi-Agent Reinforced Self-Check for LLM Hallucination

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-27  
**링크**: None

## 핵심 요약

MARCH는 LLM 환각(hallucination) 문제를 해결하기 위한 다중 에이전트 강화학습 프레임워크다. 기존 LLM-as-a-judge 방식은 검증자가 생성자의 오류를 그대로 답습하는 **확증 편향(confirmation bias)** 문제를 가진다. MARCH는 Solver(응답 생성), Proposer(주장 분해), Checker(증거 기반 검증) 세 에이전트를 설계하고, Checker가 원본 응답을 볼 수 없도록 **의도적 정보 비대칭**을 적용하여 확증 편향을 차단한다. 다중 에이전트 강화학습(MARL)으로 공동 진화시킨 결과, 8B 파라미터 모델이 대형 상용 모델에 필적하는 환각 탐지 성능을 달성했다.

## 인사이트

1. **정보 비대칭이 핵심이다** — 검증 에이전트가 원본 출력을 보지 못하게 차단함으로써, 기존 자기검증 방식의 고질적 확증 편향 문제를 구조적으로 해결했다.
2. **역할 분리가 품질을 높인다** — 응답 생성·주장 분해·사실 검증을 별도 에이전트로 분리하여 각 단계의 전문성을 극대화하고, 강화학습을 통해 에이전트 간 협력을 최적화했다.
3. **소형 모델도 경쟁력을 가진다** — 8B 규모의 오픈소스 모델에 MARCH를 적용하면 GPT-4급 대형 모델과 비슷한 사실성 검증 성능을 달성할 수 있어, 비용 효율적 배포가 가능하다.

## 응용 가능성

1. **RAG 시스템의 신뢰성 강화** — 검색 증강 생성 파이프라인에 MARCH를 통합하면, 의료·법률·금융 등 사실 정확성이 필수인 도메인에서 환각을 대폭 줄일 수 있다.
2. **자동화된 팩트체킹 시스템** — 뉴스·소셜미디어의 허위정보 탐지 파이프라인에 다중 에이전트 검증 구조를 적용하여, 대규모 콘텐츠의 사실 여부를 자동으로 교차 검증할 수 있다.

## 추출된 엔티티

- LLM Agent
- GPT-4
- Multi-Agent System

## 추출된 개념

- Multi-Agent System
- Reinforcement Learning

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-27-MARCHMulti-AgentReinforcedSelf.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-multi-agent-video-recommenders-evolution-patterns-.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-03-31-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-03-31-bace-llm-based-code-generation-through-bayesian-an.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: Multi-Agent System, LLM Agent)
- [[sources/2026-04-05-actionparty-multi-subject-action-binding-in-genera.md]] (공통 Entity: Multi-Agent System, LLM Agent)
