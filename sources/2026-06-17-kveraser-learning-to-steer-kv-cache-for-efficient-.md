# KVEraser: Learning to Steer KV Cache for Efficient Localized Context Erasing

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-17  
**링크**: http://arxiv.org/abs/2606.17034v1

## 핵심 요약

Post-hoc context erasing over the KV cache is challenging because a local edit has a global consequence: once a span has been processed, its influence propagates into the cached states of all subsequent tokens. This issue arises naturally in long-context LLM applications, where stale retrieved facts, incorrect tool observations, retracted user preferences, or harmful prompt injections may be identified only after prefill. Exact erasing must then recompute all tokens after the deleted span, makin...

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

- → [[sources/2026-06-17-tokenpilot-cache-efficient-context-management-for-]]: 둘 다 LLM 에이전트의 긴 컨텍스트 처리 과정에서 발생하는 메모리(KV 캐시) 비용 문제를 해결하기 위해 컨텍스트를 효율적으로 관리하는 방법을 제안함.
