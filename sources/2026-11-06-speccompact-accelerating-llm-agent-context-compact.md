# SpecCompact: Accelerating LLM Agent Context Compaction with Slot-Parallel Semantic Speculative Verification

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-11-06  
**링크**: http://arxiv.org/abs/2611.06876v1

## 핵심 요약

LLM agents use context compaction to manage growing interaction histories, but summarizing long histories with large models can introduce substantial delays. Compaction therefore requires balancing information retention against latency. We observe that structured summary slots can retain information when generated independently. Based on this observation, we present SpecCompact, a framework that accelerates compaction through slot-parallel semantic speculation. SpecCompact fine-tunes a small dra...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

- [[LLM Agent]]

## 추출된 개념

_없음_

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-05-you-dont-need-long-context]]: 둘 다 LLM 에이전트의 컨텍스트 압축을 다루며, SpecCompact는 '짧은 컨텍스트 유지로도 충분하다'는 전략의 핵심 병목인 컴팩션 지연을 슬롯 병렬 추측 검증으로 가속한다.
- → [[sources/2026-11-05-adversarial-speculative-reasoning-improves-long-ho]]: 속도 최적화 도구로 여겨지던 추측(speculation) 기법을 에이전트 추론 행동의 개선과 컴팩션 검증의 병렬화로 각각 재해석해 활용한다.
