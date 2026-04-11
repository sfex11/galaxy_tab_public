# SKILL0: In-Context Agentic Reinforcement Learning for Skill Internalization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-04
**링크**: http://arxiv.org/abs/2604.02268v1

## 💡 핵심 인사이트

에이전트 스킬을 추론 시점의 컨텍스트 주입이 아닌 강화학습을 통해 모델 파라미터에 내재화함으로써, 검색 노이즈와 토큰 오버헤드 없이 진정한 지식 습득을 달성할 수 있다.

## 📖 분석

## SKILL0: In-Context Agentic Reinforcement Learning for Skill Internalization

SKILL0는 LLM 에이전트의 스킬 활용 패러다임을 근본적으로 전환하는 연구다. 기존 에이전트 시스템은 추론 시점에 스킬(절차적 지식과 실행 리소스의 구조화된 패키지)을 동적으로 로드하여 컨텍스트에 주입하는 방식을 사용해왔다. 그러나 이 접근법은 검색 노이즈로 인한 무관한 가이던스 유입, 주입된 스킬 콘텐츠의 토큰 오버헤드, 그리고 모델이 지식을 실제로 '습득'하지 못하고 단순히 '따르기만' 한다는 본질적 한계를 지닌다.

SKILL0는 강화학습을 통해 스킬을 모델 파라미터에 내재화(internalization)하는 방법을 제안한다. 이는 [[knowledge-injection]]과 [[post-training]]의 교차점에 위치하며, 에이전트가 외부 도구에 의존하지 않고 내재적 역량으로 스킬을 발휘할 수 있게 한다.

이 연구는 [[llm-agent]] 엔티티의 핵심 발전 방향을 보여준다. 기존의 도구 사용(tool-use) 패러다임이 외부 리소스 검색에 의존했다면, SKILL0는 학습된 행동 패턴으로의 전환을 시도한다. [[metacognition]] 관점에서 Act Wisely 연구가 에이전트의 메타인지적 도구 선택을 다뤘다면, SKILL0는 도구 자체를 불필요하게 만드는 더 근본적인 접근이다. [[reinforcement-learning]]을 에이전트 스킬 학습에 적용한다는 점에서 Android Coach의 온라인 에이전트 훈련 효율화 연구와도 맥을 같이한다.

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Android Coach: Improve Online Agentic Training Effi
- AgentFactory: A Self-Evolving Framework Through Executable S
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- Cram Less to Fit More: Training Data Pruning Improves Memori

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/post-training.md|post-training]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/prompt-engineering.md|prompt-engineering]]

---
_LLM 분석으로 재생성됨_
