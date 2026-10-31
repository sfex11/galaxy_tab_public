# Gym-Anything for Robotics: Scaling physical simulations with digital agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40565v1

## 💡 핵심 인사이트

체화 AI의 시뮬레이션 부족은 전문가 노력 의존성이라는 제작 비용 구조의 문제이며, 코딩 에이전트가 시뮬레이션 코드를 생성하게 함으로써 환경 공급이 확장 가능한 소프트웨어 공정으로 전환된다.

## 📖 분석

Gym-Anything for Robotics는 [[agent-environment-generation]] 원리의 물리 도메인 확장이다. 원래 Gym-Anything(2026-04)이 소프트웨어를 에이전트 환경으로 변환했다면, 본 논문은 한 단계 나아가 코딩 에이전트가 물리 시뮬레이션 코드 자체를 저자하게 만든다. 체화 AI 훈련의 병목을 시뮬레이션의 태스크·물리 현상 커버리지 협소성으로 진단하되, 그 근원을 '제작이 전문가 노력에 의존해 확장 불가능한' 비용 구조로 특정한다 — [[environment-absence-bottleneck]]의 물리 도메인 정밀 진단이다. 해법은 시뮬레이션을 코드 아티팩트로 재정의하는 것으로, 제작이 자동화 가능한 코드 생성 공정이 되어 대규모 환경 공급이라는 [[environment-composition-scaling-law]]·[[scaling-laws]] 논의의 전제를 충족한다. 디지털 에이전트가 물리 시뮬레이션을 생산하는 이 역방향 구조는 [[coding-agent-domain-deboundarying]]의 극단적 사례이며, [[sim-to-real-validation-infrastructure]]의 생산 방식을 수작업 제작에서 생성 공정으로 전환한다. [[environment-capability-causality]] 관점에서 현실 전이 가능한 체화 능력의 상한이 환경 커버리지에 의해 결정됨을 재확인하고, [[embodied-ai]] 연구의 병목이 모델 능력에서 환경 인프라로 이동하고 있음을 시사한다.

## 🔗 관련 논문

- Gym-Anything: Turn any Software into an Agent Environment

## 🏷️ 엔티티

- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[entities/coding-agent-domain-deboundarying.md|coding-agent-domain-deboundarying]]
- [[entities/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]
- [[entities/embodied-ai.md|embodied-ai]]

## 📐 개념

- [[concepts/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[concepts/environment-capability-causality.md|environment-capability-causality]]
- [[concepts/environment-composition-scaling-law.md|environment-composition-scaling-law]]
- [[concepts/environment-synthesis-as-data-curation.md|environment-synthesis-as-data-curation]]
- [[concepts/scaling-laws.md|scaling-laws]]

---
_LLM 분석으로 생성됨_
