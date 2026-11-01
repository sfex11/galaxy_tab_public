# On the Fundamental Limits of Prefill-Based Decoding Length Prediction

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-11-01  
**링크**: http://arxiv.org/abs/2610.40541v1

## 핵심 요약

Predicting how many tokens a large language model (LLM) will decode, using only prefill-phase hidden states, is a key primitive for inference scheduling. We show that current benchmarks conflate predictor quality with task hardness: when the target model, dataset, or sampling configuration changes, reported accuracy collapses even though the predictor is unchanged. We trace this instability to an overlooked error source---the inherent stochasticity of autoregressive decoding---and derive bounds ...

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

---
**관련**: [[entities/predictor-hardness-conflation.md|predictor hardness conflation]]

---
**관련**: [[entities/decoder-primitive-redefinition.md|decoder primitive redefinition]]

---
**관련**: [[concepts/predictor-hardness-conflation.md|predictor hardness conflation]]
