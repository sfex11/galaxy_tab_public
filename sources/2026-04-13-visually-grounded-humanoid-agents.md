# Visually-grounded Humanoid Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08509v1

## 💡 핵심 인사이트

디지털 휴먼을 privileged state 없이 시각 관측과 목표 지정만으로 능동적으로 행동하게 함으로써, 임의의 새로운 3D 환경에 자연스러운 디지털 휴먼을 대규모로 배치할 수 있는 확장성을 확보했다.

## 📖 분석

## Visually-grounded Humanoid Agents

본 논문은 디지털 휴먼 생성의 패러다임을 **수동적 애니메이션(passive animation)**에서 **능동적 시각 기반 행동(active visually-grounded behavior)**으로 전환하는 연구다. 기존 디지털 휴먼 시스템은 privileged state 정보나 스크립트 기반 제어에 의존하여 새로운 환경으로의 확장성이 제한되었다. 이 연구는 시각 관측(visual observation)과 목표 지정(goal specification)만으로 3D 환경에서 자발적이고 자연스러운 행동을 하는 휴머노이드 에이전트를 제안한다.

### 기존 Wiki와의 관계

- **[[humanoid-agent]]**: 이 논문의 직접적 후속 버전(v1)으로, 기존 2026-04-11/12 엔트리와 동일 연구선상에 있다. 시각 기반 휴머노이드 에이전트의 핵심 프레임워크를 정의한다.
- **[[visual-locomotion]]**: 시각 정보만으로 이동을 수행하는 핵심 능력과 직결된다.
- **[[embodied-ai]]**: privileged state 없이 시각 관측 기반으로 환경과 상호작용하는 embodied AI의 대표 사례다.
- **[[3d-human-reconstruction]]**: 디지털 휴먼 생성 파이프라인의 렌더링/재구성 단계와 연결된다.
- **[[vision-language-model]]**: 목표 지정(goal specification)에 VLM 기반 접근이 활용될 가능성이 높다.

### 핵심 기여

수동적 제어에서 능동적 시각 기반 에이전트로의 전환은 **scalability** 문제를 해결하며, 임의의 3D 환경에 디지털 휴먼을 대규모로 배치(populate)할 수 있는 가능성을 열었다. 이는 강화학습 기반 locomotion 정책과 시각 인식을 결합한 접근으로, [[reinforcement-learning]]과 [[visual-grounding]] 개념의 교차점에 위치한다.

## 🔗 관련 논문

- 2026 04 11 visually grounded humanoid agents
- 2026 04 12 visually grounded humanoid agents

## 🏷️ 엔티티

- [[entities/vlm.md|VLM]]
- [[entities/mllm.md|MLLM]]

## 📐 개념

- [[concepts/humanoid-agent.md|humanoid-agent]]
- [[concepts/visual-locomotion.md|visual-locomotion]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/3d-human-reconstruction.md|3d-human-reconstruction]]
- [[concepts/vision-language-model.md|vision-language-model]]
- [[concepts/visual-grounding.md|visual-grounding]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/goal-conditioned-policy.md|goal-conditioned-policy]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-12-visually-grounded-humanoid-agents]]: 동일 논문의 다른 날짜 요약으로, 시각 기반 휴머노이드 에이전트를 다룬다.
