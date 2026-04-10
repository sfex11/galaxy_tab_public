# NavTrust: Benchmarking Trustworthiness for Embodied Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-21
**링크**: http://arxiv.org/abs/2603.19229v1

## 💡 핵심 인사이트

체화된 내비게이션 에이전트의 평가를 이상적 조건의 성능 측정에서 실세계 입력 손상에 대한 신뢰성 평가로 확장하여, 안전한 실배포를 위한 벤치마크 패러다임을 제시한다.

## 📖 분석

## NavTrust: Benchmarking Trustworthiness for Embodied Navigation

NavTrust는 체화된 내비게이션(Embodied Navigation) 시스템의 **신뢰성(trustworthiness)**을 체계적으로 평가하기 위한 통합 벤치마크이다. 기존 연구들이 이상적인 조건에서의 성능만 평가해온 한계를 지적하며, 실제 환경에서 발생할 수 있는 다양한 입력 손상(corruption)에 대한 강건성을 측정한다.

### 핵심 구조

NavTrust는 체화된 내비게이션의 두 주요 범주를 모두 다룬다:
- **Vision-Language Navigation (VLN)**: 자연어 지시를 따라 내비게이션하는 에이전트
- **Object-Goal Navigation (OGN)**: 지정된 목표 객체로 내비게이션하는 에이전트

벤치마크는 입력 모달리티(시각, 언어 등)에 체계적으로 손상을 가하여, 모델이 현실 세계의 노이즈와 불완전한 입력에 얼마나 강건한지를 평가한다. 이는 실험실 조건과 실제 배포 환경 사이의 성능 격차를 정량화하는 데 핵심적인 기여를 한다.

### 연구적 의의

NavTrust는 [[embodied-ai]] 분야에서 **평가 패러다임의 전환**을 제안한다. 단순 성능 지표(SR, SPL 등)를 넘어, 적대적·노이즈 조건에서의 신뢰성까지 벤치마크에 포함함으로써, VLN/OGN 모델의 실용적 배포 가능성을 보다 현실적으로 진단할 수 있게 한다. 이는 [[ai-safety]] 관점에서도 중요한데, 체화된 에이전트가 물리적 환경에서 동작할 때 입력 손상에 따른 오작동은 직접적인 안전 문제로 이어질 수 있기 때문이다.

기존 AgentVLN이 에이전틱 내비게이션의 능동적 탐색에 초점을 맞췄다면, NavTrust는 그러한 시스템의 **강건성과 신뢰성 평가**라는 상보적 역할을 수행한다.

## 🔗 관련 논문

- 2026 04 09 claw eval toward trustworthy evaluation of autonom
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]

---
_LLM 분석으로 재생성됨_
