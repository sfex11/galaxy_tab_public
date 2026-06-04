# NetKV: Network-Aware Decode Instance Selection for Disaggregated LLM Inference

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-04  
**링크**: http://arxiv.org/abs/2606.03910v1

## 핵심 요약

Disaggregated LLM inference forces the KV cache to traverse the datacenter network before decoding begins, so transfer time enters directly into the Time to First Token (TTFT) budget. Current schedulers route on compute load and prefix-cache locality alone, ignoring the topological distance and dynamic congestion between prefill and decode instances. We close this gap with a thin operator-to-scheduler interface, the network cost oracle, and we prove that ignoring the network term renders cache-a...

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
