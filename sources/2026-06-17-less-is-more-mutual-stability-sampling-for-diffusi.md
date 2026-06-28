# LESS Is More: Mutual-Stability Sampling for Diffusion Language Models

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-06-17  
**링크**: http://arxiv.org/abs/2606.16908v1

## 핵심 요약

Diffusion large language models (dLLMs) offer a promising alternative to autoregressive decoding by iteratively refining masked sequences, enabling parallel token updates and bidirectional conditioning. Their practical efficiency, however, is limited by sampling procedures that execute a fixed number of reverse denoising steps selected before decoding, spending computation on already-stable positions and sometimes committing unstable ones too early. We present \textsc{LESS}, a training-free, mod...

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

- → [[sources/2026-06-17-follow-the-latent-roadmap-navigating-revocable-dec]]: 둘 다 디퓨전 언어 모델(dLLM)의 디코딩 품질과 효율성을 개선하는 새로운 샘플링 및 디코딩 전략을 제안함.
- → [[sources/2026-06-18-learning-from-the-self-future-on-policy-self-disti]]: 둘 다 디퓨전 언어 모델(dLLM)의 효율성과 품질 개선을 목표로 하는 포스트 트레이닝 또는 샘플링 방법을 제안함.
- → [[sources/2026-06-19-diffusion-proof-recipe-for-formal-theorem-proving-]]: 둘 다 디퓨전 언어 모델(dLLM)의 병렬 생성 및 반복적 정제(refinement) 능력을 활용하여 특정 도메인의 출력 품질을 향상시킴.

---
**관련**: [[concepts/rollout-budget-convergence-efficiency.md|rollout budget convergence efficiency]]

---
**관련**: [[concepts/autoregressive-paradigm-confinement.md|autoregressive paradigm confinement]]

---
**관련**: [[concepts/strategic-convergence-condition.md|strategic convergence condition]]

---
**관련**: [[concepts/position-invariant-kv-reuse.md|position invariant kv reuse]]
