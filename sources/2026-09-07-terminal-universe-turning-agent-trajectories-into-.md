# Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04148v1

## 💡 핵심 인사이트

궤적은 동결된 단일 데모지만 그 도구 실행 이력은 환경 구조를 노출하며, 이를 환경으로 재질의하면 경험이 소모성 데이터에서 재사용 가능한 학습 인프라로 전환된다.

## 📖 분석

Terminal-Universe는 축적된 터미널 에이전트 궤적을 사후학습용 실행 환경으로 변환하는 시스템이다. 핵심은 궤적과 환경의 위상 차이다 — 궤적은 단일 동결 데모에 불과하지만, 환경은 검증 가능한 다수 태스크로 재질의(re-query)할 수 있고 실행 피드백을 제공하는 학습 프리미티브다. 변환 메커니즘은 궤적 내 도구 실행 이력이 환경 구조를 이미 노출한다는 관찰에 있으며, 이는 환경 부재 병목([[environment-absence-bottleneck]])이 환경 제작 능력이 아닌 '환경화 관점'의 결여에서 비롯됨을 보여준다.

Wiki와의 관계: (1) [[experience-infrastructuralization]] 개념의 최초 실현 — 궤적을 RLVR 소모성 데이터로 소비하는 대신 [[re-queryable-environment]] 인프라로 재질화한다. (2) SkillOS의 스킬 추출과 별도의 궤적 재활용 축을 개척하여 [[skill-consumption-gap]]에 환경 합성이라는 대안 경로를 제시한다. (3) [[refreshable-signal-layer]]의 훈련 측 경로로서 Claw-Eval-Live(평가 신호 갱신)·Environment Evolution(환경 도전성 갱신)과 함께 신호 지속성의 삼축을 형성한다. (4) [[self-trajectory-environment-closed-loop]]를 완성하여 자기 궤적→환경→재훈련 순환이 [[bootstrap-paradox]](자기 생성 환경으로 인한 분포 고착 위험)를 수반함을 구조적으로 제기한다. (5) [[environment-capability-causality]]를 강화한다: 궤적은 이미 축적되어 있었으므로 실질 병목은 데이터 부재가 아닌 변환 파이프라인 부재였다.

## 🔗 관련 논문

- Environment Evolution for Terminal Agents
- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Claw-Eval-Live: A Live Agent Benchmark for Evolving Real-Wor
- Gym-Anything: Turn any Software into an Agent Environment

## 🏷️ 엔티티

- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/experience-generation.md|experience-generation]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[entities/bootstrap-paradox.md|bootstrap-paradox]]
- [[entities/rlvr.md|rlvr]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-capability-causality.md|environment-capability-causality]]
- [[entities/refreshable-signal-layer.md|refreshable-signal-layer]]
- [[entities/skill-consumption-gap.md|skill-consumption-gap]]

## 📐 개념

- [[concepts/trajectory-to-environment-derivation.md|trajectory-to-environment-derivation]]
- [[concepts/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[concepts/re-queryable-environment.md|re-queryable-environment]]
- [[concepts/self-trajectory-environment-closed-loop.md|self-trajectory-environment-closed-loop]]
- [[concepts/experience-infrastructuralization.md|experience-infrastructuralization]]
- [[concepts/failure-embedded-difficulty-distribution.md|failure-embedded-difficulty-distribution]]

---
_LLM 분석으로 생성됨_
