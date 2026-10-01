# AdviSD: Learning to Advise Frontier LLMs via Targeted Multi-Turn Self-Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38142v1

## 💡 핵심 인사이트

교정이 실행을 바꾸지 않아도 학습은 다른 맥락의 미래 결정을 변화시키며, 공유 파라미터 하에서는 유용 조언을 선호하는 교정조차 학습을 제한할 수 있으므로, 조언 계층의 학습에는 표적화된 증류와 파라미터 분리가 필요하다.

## 📖 분석

AdviSD는 동결된 프론티어 LLM 실행기를 자연어 조언으로 조종하는 소형 학습형 어드바이저를 제안한다. 어드바이저는 태스크 보상에 더해 완료된 상호작용의 피드백으로부터 표적화된 다중 턴 자기 증류로 학습된다.

세 가지 통찰이 Wiki에 추가된다. 첫째, 그럴듯한 교정이 당장의 실행을 바꾸지 않아도 그 교정으로부터의 학습은 다른 맥락의 어드바이저 결정을 변화시킨다 — 교정의 행동 중립성이 학습 중립성을 의미하지 않는다는 명제로, 학습 신호가 개별 인스턴스가 아닌 분포 수준에서 작동함을 정식화한다. 둘째, 공유 파라미터 모델에서 교정 타겟이 유용한 조언을 선호하면 학습이 오히려 제한될 수 있음을 증명하여, 다중 학습 신호 공존의 조건으로 파라미터 분리를 제기한다. 셋째, 학습되지 않는 하네스와 동결 가중치 사이에 '학습되는 조언 계층'이라는 제3 구간을 연다.

[[elicitation-as-harness-artifact]]가 유도 프롬프트를 인간이 설계한 하네스 아티팩트로 보았다면, AdviSD는 그 유도 메커니즘 자체를 학습하는 후속 경로다. [[llm-as-coach]]·[[coach-actor-decoupling]]의 코칭 패러다임에 '동결 실행기+학습 코치'의 단측 학습 구성을 추가하며, [[self-retiring-distillation]]의 교사 은퇴와 대비되는 지속 조언 구조를 제시한다.

## 🔗 관련 논문

- Learning to Coach for Experiential Learning
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcem
- Harness Learning Enables Generalizable Test-Time Adaptation
- User Model Extraction via Belief Self-Distillation
- The Router Within: Eliciting Native Skill Routing from a Fro

## 🏷️ 엔티티

- [[entities/advisd.md|advisd]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/self-retiring-distillation.md|self-retiring-distillation]]
- [[entities/llm-as-coach.md|llm-as-coach]]
- [[entities/coach-actor-decoupling.md|coach-actor-decoupling]]
- [[entities/capability-internalization.md|capability-internalization]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/harness-as-capability-translator.md|harness-as-capability-translator]]

## 📐 개념

- [[concepts/harness-as-nonparametric-policy-layer.md|harness-as-nonparametric-policy-layer]]
- [[concepts/elicitation-as-harness-artifact.md|elicitation-as-harness-artifact]]
- [[concepts/thought-action-separation.md|thought-action-separation]]
- [[concepts/trajectory-as-coaching-signal.md|trajectory-as-coaching-signal]]
- [[concepts/improvement-delegation.md|improvement-delegation]]
- [[concepts/agent-as-harness.md|agent-as-harness]]
- [[concepts/gradient-interference.md|gradient-interference]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]
- [[concepts/post-training.md|post-training]]
- [[concepts/belief-self-distillation.md|belief-self-distillation]]

---
_LLM 분석으로 생성됨_
