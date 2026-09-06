# Environment Evolution for Terminal Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04128v1

## 💡 핵심 인사이트

프론티어 모델의 능력 성장이 정적 환경 합성의 학습 신호를 구조적으로 고갈시키므로, 환경은 온폴리시 롤아웃에 구속되지 않고 지속적으로 진화하는 갱신 가능 계층이 되어야 한다.

## 📖 분석

## Environment Evolution for Terminal Agents (2026-09-06)

터미널 에이전트 훈련을 위한 상호작용적·검증 가능 환경의 스케일링 문제를 다룬다. 핵심 진단은 ceiling-performance-problem의 훈련 환경 버전이다: 프론티어 모델이 강해질수록 처음부터 합성된 환경은 도전적이지 않아 학습 신호가 구조적으로 고갈되며, 검증 가능성 유지와 난이도 재조정의 양립이 [[rlvr]] 인프라의 핵심 병목으로 부상한다.

최근 공진화(co-evolution) 접근이 롤아웃에서 노출된 약점에 기반해 모델의 학습 가능 경계 근처에서 환경을 반복 합성함을 정리하되, 이들의 온폴리시 롤아웃 의존성이 일반화와 지속적 학습 신호 공급을 동시에 제한한다고 비판한다.

이는 [[agent-environment-generation]]의 스코프를 3단계로 확장한다 — Gym-Anything의 정적 소프트웨어→환경 변환, Nemobot Games의 도메인 특화 생성에 이어, '환경이 모델과 함께 지속 진화하는' 제3단계를 제시한다. 환경은 한 번 구축되는 자산이 아니라 학습 신호를 재생산해야 하는 갱신 가능 계층([[refreshable-signal-layer]]의 훈련 측 아날로그)이 된다.

[[environment-absence-bottleneck]]의 진화된 형태도 제공한다: 환경이 존재해도 모델 능력 대비 도전성이 부족하면 학습 루프는 여전히 차단되며, 이는 '부재'가 아닌 '신호 피로'에 의한 병목이다. SafeEvolve의 하네스-정책 공진화와 함께, [[environment-capability-co-evolution]]이 온폴리시 구속에서 벗어나려는 2026년 9월의 흐름을 형성한다.

## 🔗 관련 논문

- Gym-Anything: Turn any Software into an Agent Environment
- Nemobot Games: Crafting Strategic AI Gaming Agents for Interactive Learning
- SafeEvolve: Harness-Policy Co-Evolution from Agent Experience
- Terminal Universe: Turning Agent Trajectories into Environments
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-World Workflows

## 🏷️ 엔티티

- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[entities/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[entities/rlvr.md|rlvr]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/pre-existing-data-assumption.md|pre-existing-data-assumption]]

## 📐 개념

- [[concepts/environment-frontier-drift.md|environment-frontier-drift]]
- [[concepts/on-policy-environment-coupling.md|on-policy-environment-coupling]]
- [[concepts/learning-signal-exhaustion.md|learning-signal-exhaustion]]

---
_LLM 분석으로 생성됨_
