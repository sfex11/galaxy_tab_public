# BACE: LLM-based Code Generation through Bayesian Anchored Co-Evolution of Code and Test Populations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28653v1

## 💡 핵심 인사이트

LLM 코드 생성에서 생성된 테스트를 절대적 기준으로 신뢰하는 것이 핵심 병목이며, 베이지안 앵커링을 통한 코드-테스트 공진화가 이 테스트 오라클 문제를 효과적으로 해결한다.

## 📖 분석

## BACE: Bayesian Anchored Co-Evolution of Code and Test Populations

BACE는 LLM 기반 코드 생성에서 코드와 테스트를 동시에 진화시키는 공진화(co-evolution) 프레임워크이다. 기존 멀티 에이전트 프레임워크(예: AgentCoder)가 생성된 테스트를 절대적 기준(ground truth)으로 사용하는 한계를 지적하며, 이로 인해 잘못된 코드가 결함 있는 테스트를 통과하거나 올바른 코드가 잘못된 assertion에 맞춰 퇴화하는 문제를 해결한다.

BACE의 핵심은 베이지안 앵커링(Bayesian Anchoring) 메커니즘으로, 코드-테스트 간 상호 검증 시 확률적 신뢰도를 부여하여 잘못된 테스트에 의한 올바른 코드의 퇴화를 방지한다. 코드 population과 테스트 population이 서로를 평가하며 공진화하는 구조는 진화 알고리즘의 적합도 평가와 유사하지만, LLM의 생성 능력을 활용하여 변이와 선택을 수행한다는 점에서 차별화된다.

이 연구는 LLM의 코드 생성 능력을 단순 생성-실행 루프를 넘어 체계적 품질 보증으로 확장하려는 흐름에 위치한다. AgentCoder 등 기존 멀티 에이전트 코드 생성 연구에서 테스트 오라클 문제(oracle problem)가 핵심 병목이었음을 실증적으로 보여주며, 베이지안 추론을 통한 불확실성 관리가 이에 대한 유효한 해법임을 제시한다. 프로세스 제어 관점에서 Box Maze의 신뢰성 보장 접근법과도 맥을 같이 하며, 코드 생성 품질 벤치마킹 측면에서 양자 코드 생성 연구와도 연결된다.

## 🔗 관련 논문

- Box Maze: A Process-Control Architecture for Reliable LLM Re
- Revisiting Quantum Code Generation: Where Should Domain Know
- AgentFactory: A Self-Evolving Framework Through Executable S
- Bilevel Autoresearch: Meta-Autoresearching Itself
- Evaluating the Reliability and Fidelity of Automated Judgmen

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/code-generation.md|code-generation]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/llm-benchmark.md|llm-benchmark]]

---
_LLM 분석으로 재생성됨_
