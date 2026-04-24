# Latent Phase-Shift Rollback: Inference-Time Error Correction via Residual Stream Monitoring and KV-Cache Steering

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-04-22  
**링크**: http://arxiv.org/abs/2604.18567v1

## 핵심 요약

Large language models frequently commit unrecoverable reasoning errors mid-generation: once a wrong step is taken, subsequent tokens compound the mistake rather than correct it. We introduce $\textbf{Latent Phase-Shift Rollback}$ (LPSR): at each generation step, we monitor the residual stream at a critical layer lcrit, detect abrupt directional reversals (phase shifts) via a cosine-similarity $+$ entropy dual gate, and respond by rolling back the KV-cache and injecting a pre-computed steering ve...

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

- → [[sources/2026-04-23-discovering-a-shared-logical-subspace-steering-llm]]: 둘 다 추론 시점에서 LLM의 추론 방향을 제어하는 스티어링 기법을 다루며, 하나는 잔차 스트림 모니터링과 KV-캐시 조향으로, 다른 하나는 자연어-기호 언어 공유 논리 부분공간 정렬로 접근한다.
