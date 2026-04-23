# NavTrust: Benchmarking Trustworthiness for Embodied Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-22
**링크**: http://arxiv.org/abs/2603.19229v1

## 💡 핵심 인사이트

NavTrust는 체화된 내비게이션 모델을 이상적 조건이 아닌 실세계 손상 시나리오에서 평가함으로써, 성능 중심 평가에서 신뢰성 중심 평가로의 전환을 제안하는 최초의 통합 벤치마크이다.

## 📖 분석

## NavTrust: Benchmarking Trustworthiness for Embodied Navigation

NavTrust는 체화된 내비게이션(Embodied Navigation) 모델의 **신뢰성(trustworthiness)**을 체계적으로 평가하기 위한 통합 벤치마크이다. 기존 연구가 이상적 조건에서의 성능만 평가한 반면, NavTrust는 실제 환경에서 발생할 수 있는 다양한 입력 손상(corruption) 시나리오를 체계적으로 도입하여 모델의 강건성을 측정한다.

### 핵심 구성

본 벤치마크는 체화된 내비게이션의 두 주요 범주를 모두 다룬다:
- **Vision-Language Navigation (VLN)**: 자연어 지시를 따라 내비게이션하는 에이전트
- **Object-Goal Navigation (OGN)**: 지정된 목표 객체로 내비게이션하는 에이전트

입력 모달리티(시각, 언어 등)에 대한 체계적 손상을 적용하여, 명목 조건과 손상 조건 간의 성능 격차를 정량화한다.

### 연구적 의의

이 연구는 [[concepts/embodied-ai.md|embodied ai]] 분야에서 모델 평가의 패러다임을 성능 중심에서 **신뢰성 중심**으로 전환할 것을 제안한다. 이는 [[concepts/ai-safety.md|ai safety]] 관점에서도 중요한데, 실제 로봇 배치 시 입력 노이즈나 센서 오류에 대한 강건성이 안전성과 직결되기 때문이다. VLN 컴포넌트는 [[concepts/vision-language-model.md|vision language model]]과 밀접하게 연관되며, 내비게이션 에이전트의 신뢰성 평가는 [[entities/llm-agent.md|llm agent]]의 실세계 배치 신뢰성 논의와도 맥락을 같이 한다.

기존 AgentVLN이 에이전트적 내비게이션의 능력 확장에 초점을 맞췄다면, NavTrust는 그러한 능력이 **얼마나 신뢰할 수 있는지**를 묻는 상보적 연구라 할 수 있다.

## 🔗 관련 논문

- 2026 04 10 cadence context adaptive depth estimation for navi
- 2026 04 10 tracesafe a systematic assessment of llm guardrail

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/vlm.md|vlm]]

## 📐 개념

- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/multimodal-learning.md|multimodal-learning]]

---
_LLM 분석으로 재생성됨_
