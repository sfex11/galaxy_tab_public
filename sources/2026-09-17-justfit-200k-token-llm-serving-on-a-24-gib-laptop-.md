# JustFit: 200K-Token LLM Serving on a 24 GiB Laptop with Just-in-Time State Management

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-09-17  
**링크**: http://arxiv.org/abs/2609.17475v1

## 핵심 요약

Capable open-weight models make local coding and reasoning attractive, but their context and execution state strain laptop memory. We present JustFit, an MLX-based inference runtime that combines KVExec for compressed KV execution, PhaseSwap for component residency, and StateTrans for state-preserving serving transitions. These mechanisms fuse reconstruction and coordinate just-in-time materialization and release, independently of model-weight quantization. In full-execution capacity tests on a ...

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

- → [[sources/2026-09-17-flashvector-agent-for-hierarchical-model-serving-s]]: 모델 서빙 스택의 효율화라는 동일 목표를 엣지(24GiB 노트북)와 데이터센터(계층형 추천 서빙)라는 반대 환경에서 추구한다.
- → [[sources/2026-09-17-what-breaks-under-pruning-in-smart-homes-and-when-]]: 노트북·스마트홈 같은 저사양 배포 환경에서 KV 압축·상태 관리와 프루닝이 능력 저하와 맺는 트레이드오프를 다룬다.
