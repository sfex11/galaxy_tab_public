# SKILL0: In-Context Agentic Reinforcement Learning for Skill Internalization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02268v1

## 💡 핵심 인사이트

에이전트 스킬을 추론 시점에 외부 주입하는 대신 in-context RL로 모델 파라미터에 내재화함으로써, 검색 노이즈·토큰 오버헤드·지식 비영구성 문제를 동시에 해결할 수 있다.

## 📖 분석

## SKILL0: In-Context Agentic Reinforcement Learning for Skill Internalization

SKILL0는 LLM 에이전트의 스킬(skill)을 추론 시점에 외부에서 주입하는 대신, 모델 파라미터 내부로 내재화(internalize)하는 접근법을 제안한다. 기존 스킬 증강 방식은 검색 노이즈, 토큰 오버헤드, 지식의 비영구성이라는 세 가지 근본적 한계를 갖는다. SKILL0는 in-context 강화학습을 통해 절차적 지식을 파라미터 수준에서 학습시킴으로써 이 문제를 해결한다.

이 연구는 **추론 시점 증강 vs. 학습 시점 내재화**라는 중요한 축을 제시한다. 이는 RAG와 파인튜닝의 트레이드오프와 구조적으로 유사하며, tool-use 패러다임에서 도구 의존도를 줄이는 방향의 연구로 볼 수 있다. Act Wisely(메타인지적 도구 사용)가 '언제 도구를 쓸지'를 학습한다면, SKILL0는 '도구 없이도 할 수 있도록' 지식 자체를 흡수하는 것이다.

Nemotron-Cascade 2의 cascade RL이나 post-training 연구들과 마찬가지로, 사후 학습 단계에서 RL을 활용해 모델 역량을 확장하는 흐름에 속한다. 또한 knowledge-injection 관점에서 SPA 등 합성 데이터 기반 지식 주입과도 비교할 수 있으나, SKILL0는 에이전트 행동 궤적을 통한 강화학습이라는 점에서 차별화된다.

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Nemotron-Cascade 2: Post-Training LLMs with Cascade RL and M
- AgentFactory: A Self-Evolving Framework Through Executable S
- SPA: A Simple but Tough-to-Beat Baseline for Kno
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/knowledge-distillation.md|knowledge-distillation]]
- [[concepts/post-training.md|post-training]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/federated-learning.md|federated learning]]

---
**관련**: [[entities/continual-learning.md|continual learning]]

---
**관련**: [[concepts/continual-learning.md|continual learning]]

---
**관련**: [[concepts/social-learning-dynamics.md|social learning dynamics]]

---
**관련**: [[concepts/federated-learning.md|federated learning]]

---
**관련**: [[concepts/shortcut-learning.md|shortcut learning]]

---
**관련**: [[concepts/federated-continual-learning.md|federated continual learning]]

---
**관련**: [[concepts/contrastive-learning.md|contrastive learning]]
