# Deep Noir: Autonomous Steering Discovery via Architectural Chronometry in Transformer Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20722v1

## 💡 핵심 인사이트

내부 표현의 수렴 시간과 인과적 헤드 기여라는 모델 자체의 신호를 읽으면 스티어링의 위치·강도가 자동 발견되며, 그 개입 이득은 소형이 아닌 대형 모델에서 커진다.

## 📖 분석

Deep Noir는 활성화 스티어링의 고질적 수동 병목 — 어느 레이어에서, 얼마 강하게 개입할 것인가 — 를 두 개의 내부 신호로 자동화한다: Logit Lens 수렴 시점(크로노메트리)과 인과적 헤드 기여 분석. 이는 steering-read-manipulation-duality의 조작적 실현으로, 판독 계기(Logit Lens, 헤드 어트리뷰션)가 조작 계기(스티어링)의 파라미터를 산출하는 단일 파이프라인을 완성한다. [[concepts/representation-steering.md|representation steering]] 계열이 개입의 존재와 방향을 확립했다면, 본 논문은 개입의 시간 좌표 발견을 정립한다. 주목할 결과는 스케일 의존성이다 — 1B에서 16.7pp였던 이득이 7-9B에서 21-42pp로 증가하여, 스티어링이 소형 모델의 부족분 보완이 아니라 대형 모델의 정밀 제어 기법으로 재위치화될 수 있음을 시사한다. [[concepts/residual-stream-monitoring.md|residual stream monitoring]]의 판독이 상태 진단을 넘어 개입 스케줄링 신호로 기능하는 사례로, Look Before You Leap가 내부 귀속 신호를 디코딩에 연동했다면 본 논문은 동일 원리를 스티어링 계층으로 확장한다.

## 🔗 관련 논문

- What Drives Representation Steering? A Mechanistic Case Study
- Look Before You Leap: Factual Decoding with Internal Attribution Signals
- Discovering a Shared Logical Subspace: Steering LLM Logical Reasoning
- The Router Within: Eliciting Native Skill Routing from a Frozen LLM
- Position-Aware Drafting for Inference Acceleration

## 🏷️ 엔티티

- [[entities/representation-steering.md|representation-steering]]
- [[entities/activation-steering.md|activation-steering]]
- [[entities/activation-patching.md|activation-patching]]
- [[entities/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[entities/residual-stream-monitoring.md|residual-stream-monitoring]]
- [[entities/intra-generative-intervention.md|intra-generative-intervention]]
- [[entities/architectural-chronometry.md|architectural-chronometry]]
- [[entities/logit-lens-convergence.md|logit-lens-convergence]]

## 📐 개념

- [[concepts/activation-steering-parameter-automation.md|activation steering parameter automation]]
- [[concepts/architectural-chronometry.md|architectural chronometry]]
- [[concepts/logit-lens-convergence-timing.md|logit lens convergence timing]]
- [[concepts/causal-head-level-attribution.md|causal head-level attribution]]
- [[concepts/scale-dependent-steering-gains.md|scale-dependent steering gains]]
- [[concepts/read-to-manipulate-pipeline.md|read-to-manipulate pipeline]]

---
_LLM 분석으로 생성됨_
