# Discrete Beckmann Transport Models for One-Step Language Modeling and Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15903v1

## 💡 핵심 인사이트

다단계 샘플링의 스텝 압축이 교사 증류에 의존하는 한 학생 품질은 교사로 상한 고정되므로, 시간 독립적 자율 수송 사상으로 어휘 고정점 수렴을 보장하면 교사 없이도 원스텝 생성을 직접 훈련할 수 있다.

## 📖 분석

비자회귀 생성 연구의 스텝 압축 문제에 제3의 경로를 추가한다. 기존 Wiki에서 이산 생성 가속은 두 극점으로 논의되어 왔다 — Unlocking Lossless Speedups 계열의 '샘플러 교체'(AR 분포 무변경, [[distribution-preserving-acceleration]])와 Cola DLM([[cola-dlm]])의 '분포 재설계'([[parallel-decoding]], [[diffusion-llm]]). DBTM은 이들 공통의 암묵 전제를 공격한다: 다단계 샘플링을 소수 스텝으로 압축하려면 사전학습 교사의 증류([[knowledge-distillation]])가 필요했고, 이는 학생 품질을 교사로 상한 고정하며 2단계 훈련 파이프라인 비용을 부과한다 — 패러다임 전환 비용([[paradigm-translation-cost]])이 가속의 필수 통행료였던 셈이다. 해법은 시간 독립적(time-independent) 흐름이다: 단일 자율 수송 사상의 반복 적용으로 임베딩 공간의 임의의 점이 어휘 집합(정점)의 고정점으로 수렴함이 보장되므로, 생성이 다단계 ODE 근사가 아닌 동역학계 수렴으로 정의되고 교사 없이 직접 훈련된다. 토큰이 생성의 산출물이 아니라 흡인자로서 수렴의 종착점이 된다는 위상 재정의가 핵심이며, [[discrete-diffusion]] 계보에 '교사 없는 자율 수송'이라는 축을 부여하고 언어 모델링·추론 과제에서 그 성립을 실증한다.

## 🔗 관련 논문

- Unlocking Lossless Speedups in LLMs via Discrete Diffusion
- Continuous Latent Diffusion Language Model
- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Language Models
- Flow-OPD: On-Policy Distillation for Flow Matching Models

## 🏷️ 엔티티

- [[entities/dbtm.md|dbtm]]
- [[entities/discrete-diffusion.md|discrete-diffusion]]
- [[entities/diffusion-llm.md|diffusion-llm]]
- [[entities/parallel-decoding.md|parallel-decoding]]
- [[entities/cola-dlm.md|cola-dlm]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/paradigm-translation-cost.md|paradigm-translation-cost]]
- [[entities/autoregressive-generation.md|autoregressive-generation]]
- [[entities/non-autoregressive-language-modeling.md|non-autoregressive-language-modeling]]

## 📐 개념

- [[concepts/autonomous-transport-map.md|autonomous-transport-map]]
- [[concepts/fixed-point-generation.md|fixed-point-generation]]
- [[concepts/teacher-free-step-compression.md|teacher-free-step-compression]]
- [[concepts/one-step-generation.md|one-step-generation]]
- [[concepts/time-independent-flow.md|time-independent-flow]]

---
_LLM 분석으로 생성됨_
