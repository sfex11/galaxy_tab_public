# Android Coach: Improve Online Agentic Training Efficiency with Single State Multiple Actions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07277v1

## 💡 핵심 인사이트

온라인 RL에서 단일 상태-단일 행동(SSSA) 패러다임을 단일 상태-다중 행동(SSMA)으로 전환하면, 에뮬레이터 스냅샷 기반 분기 탐색을 통해 샘플 효율성을 구조적으로 개선할 수 있다.

## 📖 분석

## Android Coach: Single State Multiple Actions로 온라인 에이전트 학습 효율 개선

본 논문은 Android 에이전트의 온라인 강화학습(RL) 훈련에서 근본적 비효율성을 진단하고 해결한다. 기존 접근법은 **Single State Single Action (SSSA)** 패러다임에 갇혀 있었다—하나의 상태에서 하나의 행동만 샘플링하고 단방향 rollout으로 정책을 업데이트하는 방식이다. 이는 에뮬레이터의 높은 지연시간과 맞물려 샘플 효율성을 크게 저하시킨다.

Android Coach는 **Single State Multiple Actions (SSMA)** 패러다임을 제안한다. 하나의 상태에서 여러 행동을 탐색하여 상태-행동 쌍의 활용도를 극대화한다. 이는 에뮬레이터 스냅샷 복원을 통해 동일 상태에서 분기 탐색을 가능케 하며, 기존 온라인 RL의 샘플 비효율성 문제를 구조적으로 해결한다.

### 기존 Wiki와의 연결

이 연구는 [[concepts/reinforcement-learning.md|reinforcement learning]] 엔티티의 에이전트 훈련 효율화 맥락에서 중요하다. 특히 [[concepts/token-efficiency.md|token efficiency]] 개념과 공명하는데, Batched Contextual Reinforcement 논문이 토큰 레벨에서 효율성을 추구했다면, Android Coach는 **상태-행동 레벨**에서의 효율성을 다룬다. [[concepts/curriculum-learning.md|curriculum learning]]과도 관련이 있으며, 탐색 전략의 체계화라는 점에서 [[concepts/meta-learning.md|meta learning]]의 탐색-활용 트레이드오프 논의와 맥을 같이한다.

[[concepts/computer-use-agent.md|computer use agent]] 및 [[concepts/web-agent-evaluation.md|web agent evaluation]] 개념과도 직접 연결된다—Android 에이전트는 GUI 기반 컴퓨터 사용 에이전트의 모바일 버전이며, ClawBench 등의 평가 프레임워크와 상호보완적이다. [[concepts/tool-use.md|tool use]] 개념에서도 에이전트가 앱 인터페이스를 도구로 활용하는 패턴을 보인다.

## 🔗 관련 논문

- Batched Contextual Reinforcement: A Task-Scaling Law for Eff
- ClawBench: Can AI Agents Complete Everyday Online Tasks?
- Comparing Human Oversight Strategies for Computer-Use Agents
- Robust Quadruped Locomotion via Evolutionary Reinforcement
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M

## 🏷️ 엔티티

- [[entities/reinforcement-learning.md|reinforcement-learning]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/computer-use-agent.md|computer-use-agent]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/curriculum-learning.md|curriculum-learning]]
- [[concepts/meta-learning.md|meta-learning]]

---
_LLM 분석으로 재생성됨_
