# SwapBot: Tool-Centric Robot Manipulation via Interchangeable End-Effectors and Tactile Sensing

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40646v1

## 💡 핵심 인사이트

물리적 도구 사용의 병목은 도구 인지 능력이 아니라 교체 가능한 하드웨어 모듈성과 접촉 피드백의 결합에 있으며, 이는 디지털 에이전트의 도구 호출 패러다임이 하드웨어 교체라는 물리적 동형물을 갖는다는 것을 보여준다.

## 📖 분석

## SwapBot: 도구 중심 로봇 조작과 모듈형 엔드이펙터

SwapBot은 교체 가능한 엔드이펙터와 촉각 감지를 결합하여 도구 중심 조작을 실현하는 모듈형 시스템이다. 일상 조작(팬 프라이두부 요리 등)이 강한 절단, 정교한 브러싱, 정밀 배치 등 이질적 도구 사용을 요구한다는 관찰에서 출발하며, 저비용 어댑터로 빠른 도구 교체를 가능하게 한다.

### Wiki와의 관계

이 논문은 [[tool-use]] 개념을 소프트웨어 에이전트에서 물리 로봇으로 확장한다. 디지털 에이전트의 API 호출에 대응하는 물리적 원시 연산이 하드웨어 어댑터를 통한 엔드이펙터 교체이며, 태스크 요구에 따른 도구 선택이 에이전트의 스킬 라우팅([[skill-space-shooting]])과 구조적으로 동형인 조합 판단임을 시사한다.

절단→브러싱→배치의 서브태스크 전이 시점에 도구 교체가 발생하므로, [[stage-transition-learning]]의 전이 판단이 하드웨어 교체 트리거로 물리화되는 새 축을 제공한다.

[[representation-action-gap]] 관점에서 촉각 감지는 시각 계획과 접촉 실행 사이의 간극을 접촉 역학 수준에서 봉합하는 감각 채널을 추가한다. 간극 해소가 표현 변환뿐 아니라 감각 다중화로도 달성될 수 있음을 보여준다.

### 연결점

- [[supernumerary-robotic-limb]](EgoThumb): 로봇 능력의 하드웨어 증강이라는 공통 축. 초과지 추가(SwapBot은 도구 교체 능력 추가)라는 점에서 하드웨어 모듈성이 능력 확장의 매체임을 상호 강화한다.
- [[latent-aligned-planning]]: 도구-태스크 매칭이 잠재 공간 정렬 문제로 재해석될 가능성을 연다.

새 인사이트: 물리적 도구 사용의 병목은 도구 인지 능력이 아니라 교체 가능한 하드웨어 모듈성과 접촉 피드백의 결합에 있을 수 있다.

## 🔗 관련 논문

- EgoThumb: A Vision-Driven Supernumerary Robotic Thumb for Autonomous G
- Skill-Space Shooting for Autonomous Robot Policy Improvement
- StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks vi
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- Show-Harness: Just a VLM Agent Can Play Robots

## 🏷️ 엔티티

- [[entities/tool-use.md|tool-use]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/representation-action-gap.md|representation-action-gap]]
- [[entities/intent-action-interface.md|intent-action-interface]]

## 📐 개념

- [[concepts/interchangeable-end-effector.md|interchangeable-end-effector]]
- [[concepts/tool-centric-manipulation.md|tool-centric-manipulation]]
- [[concepts/tactile-contact-sensing.md|tactile-contact-sensing]]

---
_LLM 분석으로 생성됨_
