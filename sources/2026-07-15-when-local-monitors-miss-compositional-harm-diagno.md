# When Local Monitors Miss Compositional Harm: Diagnosing Distributed Backdoors in Multi-Agent Systems

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-15  
**링크**: http://arxiv.org/abs/2607.11751v1

## 핵심 요약

As multi-agent, tool-using LLM systems are deployed, a common safety net is a runtime monitor that checks each message, tool call, or step on its own. We show this net has a fundamental hole. A distributed backdoor splits a harmful payload across agents, so every local check passes while the assembled object is the attack. The monitor can be right on every step and still miss the attack. The problem is not splitting itself: split fragments can still leak suspicious tokens or provenance edges. Th...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

_없음_

## 추출된 개념

- [[Multi-Agent System]]

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-07-15-paradoxes-of-game-theoretic-equilibria-and-price-o]]: 둘 다 다중 에이전트 시스템에서 기존의 국소적/정적 분석框架이 가진 근본적 한계를 다루며, 하나는 분산 백도어의 안전 감시 실패를, 다른 하나는 정적 균형 개념의 비적합성을 증명함.
- → [[sources/2026-07-17-the-dynamic-verifiable-multi-agent-human-agentic-l]]: 둘 다 다중 에이전트 시스템에서의 신뢰성 문제를 다루며, 하나는 상거래에서 인간-에이전트 충성도 루프의 검증 가능성을, 다른 하나는 분산 백도어로 인한 국소 모니터링의 실패를 다룸.
