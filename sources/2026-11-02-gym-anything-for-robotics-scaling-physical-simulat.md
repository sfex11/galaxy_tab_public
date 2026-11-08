# Gym-Anything for Robotics: Scaling physical simulations with digital agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40565v1

## 💡 핵심 인사이트

체화 AI 훈련의 근본 병목이 물리 시뮬레이션의 전문가 의존적 제작에 있음을 진단하고, 코딩 에이전트의 코드 저작 능력을 환경 공급 인프라로 전용함으로써 디지털 지능이 체화 지능의 훈련 가능성을 생산하는 역방향 의존 구조를 연다.

## 📖 분석

이 논문은 Gym-Anything 계열 환경 생성 패러다임의 물리 도메인 확장이다. 기존 [[concepts/agent-environment-generation.md|agent environment generation]]이 소프트웨어를 에이전트 환경으로 변환했다면, 본 논문은 코딩 에이전트가 로봇 시뮬레이션 자체를 저작하여 체화 AI 훈련의 환경 병목을 공략한다. 시뮬레이션 제작이 전문가 노력에 의존해 확장 불가능하다는 진단([[concepts/environment-absence-bottleneck.md|environment absence bottleneck]])에 대해, 디지털 에이전트의 코드 저작 능력을 환경 공급 인프라로 전용하는 해법을 제시한다. 본 논문은 [[concepts/coding-agent-domain-deboundarying.md|coding agent domain deboundarying]]('코딩 에이전트 = 소프트웨어 전용' 구획의 붕괴)과 [[concepts/sim-to-real-validation-infrastructure.md|sim to real validation infrastructure]]의 원천 사례로서, 물리 시뮬레이션이 [[concepts/environment-as-training-primitive.md|environment as training primitive]]로 격상됨을 보여준다. 디지털 지능이 체화 지능의 훈련 환경을 생산하는 역방향 의존 구조([[concepts/environment-capability-causality.md|environment capability causality]])는 환경 생성이 LLM 에이전트와 로보틱스 양 진영을 잇는 공유 인프라임을 확정하며, [[concepts/environment-composition-scaling-law.md|environment composition scaling law]] 관점에서 시뮬레이션의 태스크·물리 다양성 구성이 체화 모델 능력의 상한을 결정하는 새 스케일링 축을 연다. [[concepts/environment-supply-scaling.md|environment supply scaling]]의 병목이 인적 자원에서 에이전트 능력으로 이동했음을 시사한다.

## 🔗 관련 논문

- Gym-Anything for Robotics: Scaling physical simulations with digital agents
- Scaling Laws for Tool-Use Agents via Controllable Environment Synthesis
- EnvSched: Environment-Aware Scheduling for Rollout-Efficient Agent Rei

## 🏷️ 엔티티

- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/coding-agent-domain-deboundarying.md|coding-agent-domain-deboundarying]]
- [[entities/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[entities/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[entities/environment-capability-causality.md|environment-capability-causality]]
- [[entities/environment-composition-control.md|environment-composition-control]]
- [[entities/environment-supply-scaling.md|environment-supply-scaling]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/robotics-foundation-model.md|robotics-foundation-model]]
- [[entities/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]

## 📐 개념

- [[concepts/environment-composition-scaling-law.md|environment-composition-scaling-law]]
- [[concepts/environment-synthesis-as-data-curation.md|environment-synthesis-as-data-curation]]

---
_LLM 분석으로 생성됨_
