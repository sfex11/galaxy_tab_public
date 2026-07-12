# FreqDepthKV: Frequency-Guided Depth Sharing for Robust KV Cache Compression in Long-Context LLM Inference

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-09  
**링크**: http://arxiv.org/abs/2607.06519v1

## 핵심 요약

Long-context LLM inference is increasingly limited by the memory and bandwidth cost of KV caches, yet aggressive compression can remove the layer-specific evidence needed for retrieval and multi-step reasoning. We introduce FreqDepthKV, an inference-time cache compression method that factorizes adjacent-layer KV states into shared low-frequency depth components and sparse high-frequency residuals. A lightweight online probe assigns attention heads to shared-depth, residual-depth, or exact cache ...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

- [[concepts/transformer.md|transformer]]

## 추출된 개념

_없음_

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-07-10-dels-spec-decoupled-long-short-contexts-for-parall]]: 두 논문은 긴 컨텍스트 LLM 추론의 효율성을 높이기 위한 방법을 제안하며, 하나는 주파수 기반 KV 캐시 압축을 통해 메모리 대역폭을 줄이고 다른 하나는 긴-짧은 컨텍스트를 분리하여 병렬 사양 디코딩을 가속한다.
- → [[sources/2026-07-10-a-hierarchical-memory-architecture-overcomes-conte]]: 두 논문은 긴 컨텍스트를 다루는 LLM의 계산적 한계를 해결하는 것을 목표로 하며, 하나는 추론 시 KV 캐시를 압축하여 메모리 비용을 줄이고 다른 하나는 계층적 메모리 아키텍처로 컨텍스트 윈도우 제한을 극복한다.
