# DecisionRank: On-Policy Distillation for Decision-Model Rerankers

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42128v1

## 💡 핵심 인사이트

교사와 학생이 선호를 표현하는 형식 자체가 다를 때(순위 목록 vs 첫 토큰 스코어), 증류의 정렬 단위를 토큰에서 아이템으로 이동하는 것이 표현 격차를 봉합하는 경로다.

## 📖 분석

DecisionRank는 생성형 LLM 교사의 랭킹 지식을, 자회귀 디코딩 없이 첫 토큰 위치의 스코어로 직접 판단을 산출하는 결정 모델(decision model) 학생에게 전이하는 온폴리시 증류 프레임워크다. 핵심 난제는 표현 격차다 — 교사는 문서 ID 시퀀스의 순위 목록으로 선호를 표현하고, 학생은 스코어로 랭킹을 결정한다. 논문은 이 격차를 증류 단위를 토큰 공간에서 아이템 공간(item-space)으로 이동시켜 해소한다.

이는 [[concepts/on-policy-distillation.md|on policy distillation]] 계보의 패러다임 간 확장이다. RetireOPD가 에이전틱 RL에서 교사 은퇴 구조를, Every Token Needs Its Own Teacher가 토큰 수준 교사 적응을 다뤘다면, 본 논문은 교사-학생이 서로 다른 출력 패러다임(생성 vs 판단)에 있을 때의 증류를 다룬다. 교사의 순차 비교라는 특권 참조를 학생의 단일 순전파 스코어로 내면화한다는 점에서 [[concepts/privileged-reliability-decoupling.md|privileged reliability decoupling]]의 증류 측 실현 사례이기도 하다.

[[concepts/representation-contract.md|representation contract]] 관점에서 교사-학생 간 형식 불일치는 번역 계약의 재협상 대상이며, 아이템 공간 증류가 그 재협상의 구체적 메커니즘이 된다. 결정 모델이 AR 디코딩 지연을 회피한다는 점에서 [[concepts/non-autoregressive-language-modeling.md|non autoregressive language modeling]]·[[concepts/latency-constrained-reasoning.md|latency constrained reasoning]] 논의와 연결되고, 이산 선택 공간의 직접 예측은 [[concepts/action-tokenization.md|action tokenization]]과 공명한다. 생성형→판별형 전환이라는 점에서 [[concepts/cross-architecture-distillation.md|cross architecture distillation]]의 확장 사례이며, 문서 ID를 교사 표현으로 쓰는 점에서 [[concepts/semantic-id-tokenization.md|semantic id tokenization]]이 증류 인터페이스로 기능함을 보여준다.

## 🔗 관련 논문

- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcem
- Every Token Needs Its Own Teacher: Multi-teacher Adaptive On-policy Se
- Position-Aware Drafting for Inference Acceleration in LLM-Based Genera
- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion

## 🏷️ 엔티티

- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/decision-model.md|decision-model]]
- [[entities/item-space-distillation.md|item-space-distillation]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]
- [[entities/cross-architecture-distillation.md|cross-architecture-distillation]]
- [[entities/non-autoregressive-language-modeling.md|non-autoregressive-language-modeling]]
- [[entities/latency-constrained-reasoning.md|latency-constrained-reasoning]]
- [[entities/action-tokenization.md|action-tokenization]]
- [[entities/token-level-teacher-adaptation.md|token-level-teacher-adaptation]]
- [[entities/semantic-id-tokenization.md|semantic-id-tokenization]]

## 📐 개념

- [[concepts/on-policy-distillation.md|on-policy-distillation]]
- [[concepts/decision-model.md|decision-model]]
- [[concepts/item-space-distillation.md|item-space-distillation]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]
- [[concepts/cross-architecture-distillation.md|cross-architecture-distillation]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[entities/harness-as-nonparametric-policy-layer.md|harness as nonparametric policy layer]]

---
**관련**: [[entities/explicit-safety-decision-learning.md|explicit safety decision learning]]

---
**관련**: [[entities/skill-space-shooting.md|skill space shooting]]

---
**관련**: [[entities/belief-space-planning.md|belief space planning]]

---
**관련**: [[concepts/decision-rule-level-safety-emergence.md|decision rule level safety emergence]]

---
**관련**: [[concepts/decisionrank.md|decisionrank]]

---
**관련**: [[concepts/systematic-divergence-as-policy-signature.md|systematic divergence as policy signature]]

---
**관련**: [[concepts/consensus-space-migration.md|consensus space migration]]

---
**관련**: [[concepts/decision-intake-transition-gap.md|decision intake transition gap]]

---
**관련**: [[concepts/surface-policy-monitoring.md|surface policy monitoring]]

---
**관련**: [[concepts/telemetry-serving-decision-gap.md|telemetry serving decision gap]]

---
**관련**: [[concepts/safety-decision-supervision.md|safety decision supervision]]

---
**관련**: [[concepts/explicit-safety-decision-learning.md|explicit safety decision learning]]

---
**관련**: [[concepts/triaxial-trace-threat-space.md|triaxial trace threat space]]
