# DeLS-Spec: Decoupled Long-Short Contexts for Parallel Speculative Drafting

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-10  
**링크**: http://arxiv.org/abs/2607.07409v1

## 핵심 요약

Speculative decoding accelerates LLM inference by drafting multiple tokens and verifying them in parallel. Block-parallel drafters such as DFlash further improve drafting efficiency by predicting an entire block in one pass, but their position-wise predictions lack explicit intra-block causal conditioning. Recent methods such as Domino and DSpark attempt to introduce such causality into block-parallel drafting, but they require training the draft model from scratch, which limits their flexibilit...

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

- → [[sources/2026-07-09-freqdepthkv-frequency-guided-depth-sharing-for-rob]]: 두 논문은 긴 컨텍스트 LLM 추론의 효율성을 높이기 위한 방법을 제안하며, 하나는 주파수 기반 KV 캐시 압축을 통해 메모리 대역폭을 줄이고 다른 하나는 긴-짧은 컨텍스트를 분리하여 병렬 사양 디코딩을 가속한다.
