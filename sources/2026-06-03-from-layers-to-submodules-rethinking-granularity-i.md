# From Layers to Submodules: Rethinking Granularity in Replacement-Based LLM Compression

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-03  
**링크**: http://arxiv.org/abs/2606.02559v1

## 핵심 요약

Post-training compression of Large Language Models (LLMs) removes entire architectural components, either deleting them or replacing them with fitted modules. Existing replacement-based methods share two design constraints: full-layer granularity and contiguous selection. We argue that this is overly restrictive: in fact, redundancy in pretrained transformers is not confined to contiguous regions, nor does it evenly distribute between Attention and FeedForward outputs, implying that different st...

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

- → [[sources/2026-06-04-netkv-network-aware-decode-instance-selection-for-]]: 두 논문 모두 LLM의 효율적인 추론을 위한 자원 최적화를 다루며, 전자는 모델 구조 압축을 통한 연산량 최적화, 후자는 분리형 추론 환경에서의 네트워크 지연 최소화를 다룹니다.
