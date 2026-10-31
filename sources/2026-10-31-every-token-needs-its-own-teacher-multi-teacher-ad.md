# Every Token Needs Its Own Teacher: Multi-teacher Adaptive On-policy Self-distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40574v1

## 💡 핵심 인사이트

증류의 감독 입도는 응답 수준을 넘어 토큰 수준까지 세분화되어야 하며, 교사의 특권 참조 노출은 각 토큰별로 적응적으로 조절되는 동적 변수다.

## 📖 분석

On-policy Self-distillation(OPSD)은 특권 참조(privileged reference)로 조건화된 교사를 구성하여 사후학습을 수행하는 방식이다. 기존 OPSD는 교사의 참조 노출을 학습 전체에서 고정하거나 응답별로만 적응시켰으나, 본 논문은 **모든 토큰이 자신만의 교사를 필요로 한다**는 명제로 감독 입도를 토큰 수준까지 세분화한다.

이는 [[on-policy-distillation]] 계열의 감독 입도 정교화 계층을 확정한다 — 학습 전체 고정 → 응답별 적응 → 토큰별 적응. [[self-retiring-distillation]]이 '언제 은퇴할까'라는 학습 시간축의 교사 역학을 제시했다면, 본 논문은 '각 토큰에서 얼마나 참조를 보여줄까'라는 생성 위치축의 교사 역학을 추가한다. [[stage-dependent-teacher-supervision]]의 스테이지 수준 적응보다 더 미세한 최소 입도 사례가 된다.

또한 [[privileged-reliability-decoupling]]과 연결된다 — 특권 참조 노출의 관리 단위가 응답을 넘어 토큰으로 세분화됨을 보여준다. [[advisd]]의 동결 실행기-어드바이저 영구 역할 분리와 대비하여, 교사 구성 자체가 토큰별 동적 계약이 될 수 있음을 시사한다. 밀집 감독의 배분 입도 문제라는 점에서 [[reward-sparsity]] 논의에도 기여한다.

## 🔗 관련 논문

- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcem
- AdviSD: Learning to Advise Frontier LLMs via Targeted Multi-Turn Self-

## 🏷️ 엔티티

- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/self-retiring-distillation.md|self-retiring-distillation]]
- [[entities/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]
- [[entities/stage-dependent-teacher-supervision.md|stage-dependent-teacher-supervision]]
- [[entities/advisd.md|advisd]]
- [[entities/reward-sparsity.md|reward-sparsity]]

## 📐 개념

- [[concepts/token-level-teacher-adaptation.md|token-level-teacher-adaptation]]
- [[concepts/on-policy-self-distillation.md|on-policy-self-distillation]]
- [[concepts/privileged-reliability-decoupling.md|privileged-reliability-decoupling]]

---
_LLM 분석으로 생성됨_
