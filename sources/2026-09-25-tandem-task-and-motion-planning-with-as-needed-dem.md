# TANDEM: Task and Motion Planning with As-Needed Demonstrations for Efficient Vision-Language-Action Model Fine-tuning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28314v1

## 💡 핵심 인사이트

로봇 데이터 수집의 병목을 인간 시연 시간에서 TAMP 커버리지 프론티어로 이동시켜, 인간을 상시 시연자에서 계획 실패 시의 온디맨드 개입점으로 격하시킨다.

## 📖 분석

로봇 파운데이션 모델 데이터 수집의 병목을 재정의한다 — 인간 텔레오퍼레이터가 로봇이 이미 자율 수행 가능한 행동까지 시연하는 낭비를 제거하고, TAMP로 자동화 가능한 구간의 궤적을 자동 생성하되 고정 계획 도메인이 장기 조작 태스크의 모든 단계를 지원하지 못하는 지점에서만 인간 시연을 '필요에 따라(as-needed)' 요청한다. 기존 Wiki와의 세 접점: 첫째 VLA 훈련 인프라 축 — VLA Foundry가 통합 훈련 프레임워크를 공급했다면 TANDEM은 데이터 획득 측에서 시연 자동화 경로를 제공하여 end-to-end VLA 훈련의 입력 병목을 완화한다. 둘째 StageGuard-SeeQ 계열과의 동형 구조 — StageGuard가 행동 단계 간 전이 경계를 학습했다면 TANDEM은 '계획 도메인 커버리지의 경계'를 판정 대상으로 삼아, 경계 감지 문제가 행동 전이에서 계획-인간 인계 지점으로 확장됨을 보여준다. 셋째 인간 역할의 재정의 — 인간이 상시 시연자에서 계획 실패 시 개입하는 온디맨드 확장점으로 이동하는 것은 computation-unit-meta-selection(SLM/LLM 라우팅)과 human-as-harness-internal-component의 로봇 도메인 발현이다. 확장 여지로, 자동화 프론티어가 학습과 함께 이동하면 환경-능력 공진화의 데이터 수집 버전이 열리고, TAMP 생성 궤적의 실행 검증 가능성은 실행 검증 계열과 연결된다.

## 🔗 관련 논문

- VLA Foundry: A Unified Framework for Training Vision-Language-Action Models
- StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks via Agentic Distillation
- SeeQ: Training Generalist Value Functions for Long-Horizon Robotic Manipulation
- Environment Evolution for Terminal Agents
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for End-to-End...

## 🏷️ 엔티티

- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/stage-transition-learning.md|stage-transition-learning]]
- [[entities/robotics-foundation-model.md|robotics-foundation-model]]
- [[entities/environment-capability-co-evolution.md|environment-capability-co-evolution]]
- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/experience-generation.md|experience-generation]]

## 📐 개념

- [[concepts/as-needed-demonstration.md|as-needed-demonstration]]
- [[concepts/planning-domain-coverage-limit.md|planning-domain-coverage-limit]]
- [[concepts/tamp-teleoperation-hybrid-data-collection.md|tamp-teleoperation-hybrid-data-collection]]
- [[concepts/demonstration-burden-automation.md|demonstration-burden-automation]]

---
_LLM 분석으로 생성됨_
