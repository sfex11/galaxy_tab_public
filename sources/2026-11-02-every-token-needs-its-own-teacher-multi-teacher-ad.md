# Every Token Needs Its Own Teacher: Multi-teacher Adaptive On-policy Self-distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40574v1

## 💡 핵심 인사이트

'모든 토큰이 자신만의 교사를 갖는다'는 원리로 교사 감독의 적응 입도가 최소 단위에 도달하며, 교사-학생 구조의 설계 공간이 고정-은퇴-동적 재구성의 삼극점으로 완성된다.

## 📖 분석

OPSD(On-policy Self-distillation)의 교사 설계에 입도 논리를 도입한다. 기존 OPSD는 교사를 훈련 전체에서 고정하거나 응답 단위로만 적응시켰으나, 본 논문은 '모든 토큰이 자신만의 교사를 필요로 한다'며 특권 참조 노출량을 토큰별로 재구성하는 다중 교사 적응 구조를 제안한다. 이는 위키의 신호 정교화 축([[concepts/adaptive-inference.md|adaptive inference]]의 추론 자원 입도, [[concepts/adaptive-credit-granularity.md|adaptive credit granularity]]의 크레딧 입도)에 병렬되는 훈련 신호 입도의 최소 단위 도달이다. 교사-학생 구조의 설계 공간이 삼극점으로 확정된다: [[entities/advisd.md|advisd]]의 동결 실행기-학습 어드바이저 영구 분리, [[concepts/self-retiring-distillation.md|self retiring distillation]]의 교사 은퇴, 그리고 본 논문의 토큰별 동적 재구성. 은퇴가 '언제 물러나는가'의 시간축이라면 본 논문은 '얼마나 세밀하게 개입하는가'의 입도축으로, 두 축이 직교하는 교사 생애주기 설계 2차원이 성립한다. 또한 교사 밀집 감독이 희소 보상을 완화하되([[concepts/reward-sparsity.md|reward sparsity]]), 감독 자체가 토큰별로 적응해야 학생 자율성 제한 비용을 최소화함을 보여준다. 특권 참조 노출 관리([[concepts/privileged-reliability-decoupling.md|privileged reliability decoupling]])가 응답 단위 제어를 넘어 토큰 단위 세밀 제어의 대상이 됨을 의미한다.

## 🔗 관련 논문

- Every Token Needs Its Own Teacher: Multi-teacher Adaptive On-policy Self-distillation
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning
- AdviSD: Learning to Advise Frontier LLMs via Targeted Multi-Turn Self-Distillation

## 🏷️ 엔티티

- [[entities/token-level-teacher-adaptation.md|token-level-teacher-adaptation]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/self-retiring-distillation.md|self-retiring-distillation]]
- [[entities/advisd.md|advisd]]
- [[entities/stage-dependent-teacher-supervision.md|stage-dependent-teacher-supervision]]
- [[entities/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]
- [[entities/reward-sparsity.md|reward-sparsity]]

## 📐 개념

- [[concepts/adaptive-credit-granularity.md|adaptive-credit-granularity]]
- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/on-policy-self-distillation.md|on-policy-self-distillation]]
- [[concepts/signal-existence-premise.md|signal-existence-premise]]

---
_LLM 분석으로 생성됨_
