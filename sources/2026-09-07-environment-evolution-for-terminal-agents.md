# Environment Evolution for Terminal Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04128v1

## 💡 핵심 인사이트

공진화 환경 진화가 온폴리시 롤아웃에 결속되면 환경은 모델 능력의 그림자를 복제할 뿐 일반화된 학습 신호를 제공하지 못한다 — 환경 진화의 진짜 과제는 능력 경계 추적이 아니라 진화 근거의 정책 독립성 확보다.

## 📖 분석

# Environment Evolution for Terminal Agents

터미널 에이전트 훈련에서 상호작용적·검증 가능 환경의 스케일링은 폐루프 훈련의 생존 조건이다. 프론티어 모델이 강해질수록 스크래치 합성 환경은 도전성을 상실하여 [[learning-signal-exhaustion]]가 발생한다. 공진화(co-evolution) 방법은 롤아웃에서 노출된 약점에 기반해 모델의 학습 가능 경계([[environment-frontier-drift]]) 부근에서 환경을 반복 합성한다.

## 핵심 진단: 온폴리시 결속의 한계
본 논문은 공진화의 구조적 한계를 규명한다: 환경 진화가 온폴리시 롤아웃에 의존하면([[on-policy-environment-coupling]]) (1) 일반화가 제한되고 (2) 학습 신호의 지속 공급이 현재 정책 분포에 결속된다. 환경이 모델 능력과 공진화하더라도([[environment-capability-co-evolution]]) 진화 근거가 정책 내부에만 있으면 환경은 능력의 그림자에 불과하다.

## 기존 Wiki와의 관계
- [[terminal-universe]]와 대비: 궤적→환경 파생(오프라인·경험 기반) vs 약점→환경 진화(온폴리시·약점 기반). 환경 공급의 두 경로는 서로의 결속 한계를 상보적으로 보완한다.
- [[refreshable-signal-layer]]: [[claw-eval-live]]의 평가측 신호 갱신에 대한 훈련측 아날로그이나, 갱신 트리거의 정책 결속성이라는 새 비판 축을 추가한다.
- [[environment-absence-bottleneck]]: 병목의 3단계 진화(환경 부재→신호 피로→피로 재발 조건)를 완성한다.
- [[closed-loop-training]]: 폐루프의 닫힘 조건이 환경 갱신 빈도뿐 아니라 갱신 데이터 소스의 정책 독립성까지 요구함을 명시한다.

## 🔗 관련 논문

- Environment Evolution for Terminal Agents
- Terminal-Universe: Turning Agent Trajectories into Scalable 
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-Wor

## 🏷️ 엔티티

- [[entities/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/pre-existing-data-assumption.md|pre-existing-data-assumption]]

## 📐 개념

- [[concepts/learning-signal-exhaustion.md|learning-signal-exhaustion]]
- [[concepts/on-policy-environment-coupling.md|on-policy-environment-coupling]]
- [[concepts/environment-frontier-drift.md|environment-frontier-drift]]
- [[concepts/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[concepts/agent-environment-generation.md|agent-environment-generation]]
- [[concepts/environment-capability-causality.md|environment-capability-causality]]

---
_LLM 분석으로 생성됨_
