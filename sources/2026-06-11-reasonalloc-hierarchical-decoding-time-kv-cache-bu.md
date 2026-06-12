# ReasonAlloc: Hierarchical Decoding-Time KV Cache Budget Allocation for Reasoning Models

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-11  
**링크**: http://arxiv.org/abs/2606.11164v1

## 핵심 요약

Long chain-of-thought (CoT) trajectories in large language model (LLM) reasoning cause severe inference bottlenecks due to rapid key-value (KV) cache growth. Current decoding-time compression methods mitigate this issue via token eviction, but typically assume a uniform budget distribution across all layers and heads. In contrast, existing non-uniform budget allocation methods are predominantly designed for the static prompt prefill phase, and they do not capture the stepwise context demands of ...

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

- → [[sources/2026-06-12-on-subquadratic-architectures-from-applications-to]]: 두 논문 모두 트랜스포머 어텐션의 이차적 계산 비용이라는 병목을 해결하며, 하나는 KV 캐시 예산 할당으로, 다른 하나는 서브이차 아키텍처 대안으로 접근합니다.
