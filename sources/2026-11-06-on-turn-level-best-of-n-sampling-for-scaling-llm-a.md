# On Turn-Level Best-of-N Sampling for Scaling LLM Agents

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-11-06  
**링크**: http://arxiv.org/abs/2611.06868v1

## 핵심 요약

In this work, we evaluate a simple inference-time scaling approach based on \textit{turn-level best-of-N sampling} (\method) for large language model (LLM) agents on complex, long-horizon tasks. We instantiate this using a \textit{generator-selector} framework with two LLMs; at each turn, a \emph{generator} model generates $N$ candidate actions and a \emph{selector} model selects one of them, which is then executed in the environment. This paper is closely related to the work of \cite{zainullina...

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

_없음_

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-06-rethinking-self-repair-in-code-as-policy-agents-wh]]: 재시도 성공의 원인이 실패별 피드백인지 단순 추가 샘플링인지 분해하는 질문과, 턴 단계 best-of-N 샘플링이 각각 에이전트의 샘플링 기반 개선 문제를 다룬다.
- → [[sources/2026-11-05-adversarial-speculative-reasoning-improves-long-ho]]: 장기 과제 에이전트에서 추론 시점 확장을 드래프트-검증 추측 구조와 생성자-선택자 best-of-N 구조로 각각 구현한다.
- → [[sources/2026-11-06-context--answer-metamodels-forecasting-llm-activat]]: 확률적 디코딩으로 답변 다양성을 얻는 비용 문제를 공유하며, 메타모델은 롤아웃 전 활성화 예측으로 best-of-N 샘플링의 비용을 우회할 가능성을 연다.
