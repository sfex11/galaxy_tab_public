# EnvSched: Environment-Aware Scheduling for Rollout-Efficient Agent Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37609v1

## 💡 핵심 인사이트

agent RL의 롤아웃 효율 병목은 환경 생성이 아니라 공급된 환경의 실행·검증에 있으며, 태스크와 환경을 공동 단위로 스케줄링하는 환경 수준 데이터 관리가 이 병목의 해소 수단이다.

## 📖 분석

EnvSched의 arXiv v1 공식 발행으로 이 엔티티의 조작적 정의가 확정된다. 실행 가능 환경이 스케일할수록 롤아웃의 생성·검증 비용이 증가하며, 유한 롤아웃 예산 하에서 이것이 agent RL의 실질 병목이 된다. EnvSched의 해법은 환경 수준 데이터 관리다 — 태스크 인스턴스를 그것을 규정하는 환경(도구·상태·전이·검증자)과 함께 조직·평가·스케줄링하는 것. 이는 [[environment-supply-scaling]] 계열이 다룬 '환경 공급 확대'의 다음 단계로, 공급량이 아니라 공급된 환경의 실행 효율이 병목임을 확정한다. Scaling Laws for Tool-Use Agents가 '무엇을 만들까'([[environment-composition-control]], [[synthesis-diversity-axes]])를 다룬다면 EnvSched는 '무엇을 언제 실행할까'를 다루어, 환경 축 스케일링 법칙이 생성 계층에서 스케줄링 계층으로 분화함을 보여준다. [[kv-streams]]가 모델 측 롤아웃 효율화(반복 프리필 병목 제거)를 담당했다면 본 논문은 환경 측 롤아웃 효율화로 시스템의 나머지 절반을 채워, agent RL 인프라가 모델과 환경 양축을 아우르는 [[training-grade-serving-class]] 구조로 완성된다. 환경이 정적 원료가 아니라 스케줄링 가능한 동적 자원으로 재정의되는 지점에서, 환경 생성([[codebase-as-learning-environment]])과 환경 실행이 동일한 훈련 인프라 위의 두 계층으로 정렬된다.

## 🔗 관련 논문

- Scaling Laws for Tool-Use Agents via Controllable Environment Synthesis
- KV-streams for Efficient Compaction in Agentic Reinforcement Learning

## 🏷️ 엔티티

- [[entities/envsched.md|envsched]]
- [[entities/environment-execution-cost-bottleneck.md|environment-execution-cost-bottleneck]]
- [[entities/rollout-environment-coupling.md|rollout-environment-coupling]]
- [[entities/environment-scheduling.md|environment-scheduling]]
- [[entities/training-grade-serving-class.md|training-grade-serving-class]]
- [[entities/rollout-budget-convergence-efficiency.md|rollout-budget-convergence-efficiency]]
- [[entities/environment-supply-scaling.md|environment-supply-scaling]]
- [[entities/scaling-laws.md|scaling-laws]]
- [[entities/kv-streams.md|kv-streams]]

## 📐 개념

- [[concepts/environment-execution-cost-bottleneck.md|environment-execution-cost-bottleneck]]
- [[concepts/environment-scheduling.md|environment-scheduling]]
- [[concepts/rollout-environment-coupling.md|rollout-environment-coupling]]
- [[concepts/rollout-budget-convergence-efficiency.md|rollout-budget-convergence-efficiency]]
- [[concepts/training-grade-serving-class.md|training-grade-serving-class]]

---
_LLM 분석으로 생성됨_
