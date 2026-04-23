# UI-Voyager: A Self-Evolving GUI Agent Learning via Failed Experience

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24533v1

## 💡 핵심 인사이트

실패 궤적을 단순 거부하지 않고 credit assignment를 통해 학습 신호로 재활용함으로써, 희소 보상 환경의 장기 호라이즌 GUI 태스크에서 에이전트의 자기진화를 가능하게 한다.

## 📖 분석

## UI-Voyager: 실패 경험으로부터 학습하는 자기진화 GUI 에이전트

UI-Voyager는 모바일 GUI 자동화를 위한 2단계 자기진화(self-evolving) 에이전트로, 기존 방법들이 실패 궤적(failed trajectories)에서 효과적으로 학습하지 못하고 장기 호라이즌 태스크에서 희소 보상(sparse reward) 하의 공헌 할당(credit assignment)이 모호한 문제를 해결한다.

**1단계 — Rejection Fine-Tuning (RFT):** 데이터와 정책의 지속적 공동 진화(co-evolution)를 가능하게 한다. 성공/실패 궤적을 수집하고, 실패 궤적을 거부(reject)하면서 성공 궤적으로 미세조정하는 반복 루프를 구성한다.

**2단계 — 실패 경험 활용:** 단순 거부를 넘어 실패 궤적에서도 학습 신호를 추출하는 것이 핵심 차별점이다. 장기 호라이즌 GUI 태스크에서 각 스텝의 기여도를 정밀하게 평가하여, 희소 보상 환경에서도 효과적인 credit assignment를 수행한다.

이 접근은 [[concepts/reinforcement-learning.md|reinforcement learning]]의 exploration-exploitation 문제와 직결되며, 특히 [[entities/llm-agent.md|llm agent]] 분야에서 에이전트의 자율적 능력 향상이라는 핵심 과제를 다룬다. Android Coach(온라인 에이전트 학습 효율화)와 유사하게 모바일 환경에서의 에이전트 훈련을 다루지만, UI-Voyager는 오프라인 실패 경험 재활용에 초점을 맞춘다는 점에서 상호보완적이다. ClawBench의 웹 에이전트 평가 관점에서도, 실패 경험 학습은 실제 배포 시 에이전트 신뢰성 향상의 핵심 메커니즘이 된다. Act Wisely의 메타인지적 도구 사용과도 연결되는데, 실패로부터의 학습은 본질적으로 에이전트의 메타인지 능력에 해당한다.

## 🔗 관련 논문

- 2026 04 10 android coach improve online agentic training effi
- 2026 04 11 clawbench can ai agents complete everyday online t
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 09 maestro adapting guis and guiding navigation with

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]
- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/agentic-vlm.md|agentic-vlm]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/web-agent-evaluation.md|web-agent-evaluation]]

---
_LLM 분석으로 재생성됨_
