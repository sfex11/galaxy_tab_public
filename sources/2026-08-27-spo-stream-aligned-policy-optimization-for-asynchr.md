# SPO++: Stream-Aligned Policy Optimization for Asynchronous Agentic RL

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-08-27  
**링크**: http://arxiv.org/abs/2608.24870v1

## 핵심 요약

Group-relative reinforcement learning waits for sibling rollouts of the same prompt, which is costly for long and variable tool-use trajectories. Single-stream Policy Optimization (SPO) removes this dependency with a persistent prompt-level value estimate, but its recipe whitens one advantage per trajectory before optimizing a token-mean actor loss. We show that trajectory centering generally does not center the token-weighted quantity consumed by the actor, and fix the mismatch by standardizing...

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

- [[Reinforcement Learning]]

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-08-27-cafe-self-improving-search-agents-need-co-evolving]]: 두 논문은 에이전트가 도구를 사용하거나 탐색하는 긴 궤적 내에서 발생하는 중간 오류를 수정하고 정책을 개선하기 위한 강화 학습 기반의 피드백 메커니즘을 다룹니다.
