# Towards Load-Aware Prefill Deflection for Disaggregated LLM Serving

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-07  
**링크**: http://arxiv.org/abs/2607.02043v1

## 핵심 요약

Disaggregated LLM serving runs prefill and decode on separate GPU pools to keep the two phases from interfering. In practice, this creates a new asymmetry: under bursty, heavy-tailed workloads prefill nodes saturate while decode nodes have compute underutilized, and on a production-style A100 cluster with 2 prefill and 2 decode nodes (2P2D), we find that prefill execution accounts for only 2-23% of P95 Time-to-First-Token (TTFT). Queuing and inter-node GPU-GPU KV-cache transfer account for the r...

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
