# SwapBot: Tool-Centric Robot Manipulation via Interchangeable End-Effectors and Tactile Sensing

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40646v1

## 💡 핵심 인사이트

도구 교체가 하드웨어 수준의 인터페이스 전환이라는 명제를 넘어, 어댑터라는 표준 물리 계약과 촉각 접지의 결합이 접촉 풍부 조작의 모듈성을 가능하게 함을 확립한다.

## 📖 분석

SwapBot은 일상 조작의 본질이 도구 사용에 있다는 진단에서 출발한다 — 팬프라이 두부 요리 하나가 강한 절단, 섬세한 브러싱, 정밀한 배치라는 상이한 힘 프로파일과 접촉 조건을 요구하듯, 단일 태스크 내부에 이미 다수의 도구 전환이 중첩되어 있다. 해법은 저비용 어댑터로 신속 교체 가능한 모듈형 엔드이펙터 시스템과 촉각 감지의 결합이다.

선행 기록(2026-10-31)이 [[concepts/intent-action-interface.md|intent action interface]]의 하드웨어 확장 — 엔드이펙터 교체가 의도-실행 인터페이스 전환의 물리적 구현 — 을 확정했다면, 이번 재분석은 세 축적 중 개념의 정의를 완성한다. [[concepts/tool-centric-manipulation.md|tool centric manipulation]]은 조작을 '로봇이 도구를 쓴다'로 재정의하는 패러다임이고, [[concepts/interchangeable-end-effector.md|interchangeable end effector]]는 어댑터를 표준화된 물리 인터페이스 계약으로 규정하며, [[concepts/tactile-contact-sensing.md|tactile contact sensing]]은 접촉 풍부 상호작용에서 힘 제어의 감각적 접지를 담당한다.

[[concepts/action-tokenization.md|action tokenization]] 관점에서 어댑터 교체는 물리 세계의 액션 토큰 전환이다 — 소프트웨어의 [[concepts/representation-contract.md|representation contract]]이 하드웨어 수준에서 실현되는 사례다. EgoThumb가 초과지 사지 추가로 실행기-태스크 정합성을 풀었다면 SwapBot은 도구 교체로 동일 문제를 해결하며, 도구 선택이 [[concepts/skill-selection-functional-split.md|skill selection functional split]]과 동형의 하드웨어 라우팅 문제임을 시사한다.

## 🔗 관련 논문

- SwapBot: Tool-Centric Robot Manipulation via Interchangeable End-Effectors and Tactile Sensing (2026-10-31)
- EgoThumb: A Vision-Driven Supernumerary Robotic Thumb for Autonomous G (2026-10-30)
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En (2026-09-07)

## 🏷️ 엔티티

- [[entities/intent-action-interface.md|intent-action-interface]]
- [[entities/tool-centric-manipulation.md|tool-centric-manipulation]]
- [[entities/interchangeable-end-effector.md|interchangeable-end-effector]]
- [[entities/tactile-contact-sensing.md|tactile-contact-sensing]]

## 📐 개념

- [[concepts/tool-centric-manipulation.md|tool-centric-manipulation]]
- [[concepts/interchangeable-end-effector.md|interchangeable-end-effector]]
- [[concepts/tactile-contact-sensing.md|tactile-contact-sensing]]
- [[concepts/action-tokenization.md|action-tokenization]]
- [[concepts/representation-contract.md|representation-contract]]

---
_LLM 분석으로 생성됨_
