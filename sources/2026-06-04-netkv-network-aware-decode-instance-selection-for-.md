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

## 🔗 교차 참조

- → [[sources/2026-06-03-from-layers-to-submodules-rethinking-granularity-i]]: 두 논문 모두 LLM의 효율적인 추론을 위한 자원 최적화를 다루며, 전자는 모델 구조 압축을 통한 연산량 최적화, 후자는 분리형 추론 환경에서의 네트워크 지연 최소화를 다룹니다.
- → [[sources/2026-06-03-simsd-simple-speculative-decoding-in-diffusion-lan]]: 두 논문 모두 LLM의 추론 지연시간(Latency)을 줄이기 위한 디코딩 최적화 기법을 제안하며, 전자는 확산 모델용 추론적 디코딩, 후자는 네트워크 지연을 고려한 디코드 인스턴스 스케줄링을 다룹니다.
- → [[sources/2026-06-05-streaming-communication-in-multi-agent-reasoning]]: 두 논문 모두 LLM 시스템의 엔드투엔드 추론 지연시간(Latency) 최소화를 다루며, 전자는 다중 에이전트 간 스트리밍 통신, 후자는 분리형 추론 아키텍처에서의 네트워크 전송 시간 최소화를 다룹니다.

---
**관련**: [[concepts/pre-decoding-refusal-detection.md|pre decoding refusal detection]]

---
**관련**: [[concepts/composition-operator-alignment.md|composition operator alignment]]

---
**관련**: [[concepts/dynamic-lifecycle-safety.md|dynamic lifecycle safety]]
