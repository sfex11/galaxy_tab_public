# Kamera: Unified Position-Invariant Multimodal KV Cache for Training-Free Reuse

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-24  
**링크**: http://arxiv.org/abs/2606.23581v1

## 핵심 요약

Multimodal agents repeatedly re-examine the same video frames, UI screenshots, and rendered artifacts as their context window slides and reasoning iterates, yet every look-back re-encodes from scratch, because prefix caches serve reuse only at a fixed leading position. We show this recompute is avoidable, and identify exactly what naive KV reuse loses: the cross-chunk conditioning a chunk absorbs from its neighbours. This loss is asymmetric. The direct readout of a cached chunk is recovered exac...

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

- → [[sources/2026-06-24-randomized-yarn-improves-length-generalization-for]]: 둘 다 LLM이 긴 컨텍스트를 처리할 때의 효율성과 일반화 문제를 해결하며, 하나는 위치 불변 KV 캐시 재사용으로 재계산을 줄이고, 다른 하나는 랜덤화 YaRN으로 길이 일반화를 개선함.
