# TokenPilot: Cache-Efficient Context Management for LLM Agents

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-17  
**링크**: http://arxiv.org/abs/2606.17016v1

## 핵심 요약

As LLM agents are deployed in long-horizon sessions, context accumulation drives up inference costs. Existing approaches utilize text pruning or dynamic memory eviction to minimize token footprints; however, their unconstrained sequence mutations alter layouts, introducing prefix mismatches and cache invalidation. This reveals a critical trade-off between text sparsity and prompt cache continuity. To address this, we present TokenPilot, a dual-granularity context management framework. Globally, ...

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

- → [[sources/2026-06-17-kveraser-learning-to-steer-kv-cache-for-efficient-]]: 둘 다 LLM 에이전트의 긴 컨텍스트 처리 과정에서 발생하는 메모리(KV 캐시) 비용 문제를 해결하기 위해 컨텍스트를 효율적으로 관리하는 방법을 제안함.

---
**관련**: [[concepts/mutation-authority-separation.md|mutation authority separation]]
