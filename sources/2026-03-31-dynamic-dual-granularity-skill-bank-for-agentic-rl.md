# Dynamic Dual-Granularity Skill Bank for Agentic RL

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28716v1

## 💡 핵심 인사이트

에이전트 RL에서 경험 재사용을 태스크/스텝 이중 세분화로 조직하고 정책과 공동 학습하는 동적 스킬 뱅크가 기존 정적·단일 수준 스킬 추출의 한계를 극복한다.

## 📖 분석

## Dynamic Dual-Granularity Skill Bank for Agentic RL (D2Skill)

D2Skill은 에이전트 강화학습에서 재사용 가능한 경험을 **이중 세분화(dual-granularity)** 구조로 조직하는 동적 스킬 뱅크를 제안한다. 핵심은 태스크 스킬(고수준 가이드)과 스텝 스킬(세밀한 의사결정 및 오류 수정)을 분리하여 관리하는 것이다.

### 기존 Wiki와의 관계

**[[concepts/reinforcement-learning.md|reinforcement learning]]**과 직접 관련되며, 특히 스킬 기반 RL의 한계(궤적 수준 가이드만 추출, 진화하는 스킬 메모리 관리 메커니즘 부재)를 해결한다. **[[concepts/hierarchical-representation.md|hierarchical representation]]** 개념과 유사하게, 경험을 계층적으로 구조화하여 고수준/저수준 의사결정을 분리한다.

**[[concepts/metacognition.md|metacognition]]** 및 **[[concepts/tool-use.md|tool use]]**와도 연결된다. 스텝 스킬의 오류 수정 기능은 에이전트가 자신의 행동을 모니터링하고 교정하는 메타인지적 특성을 가지며, Act Wisely(2026-04-11) 논문의 메타인지적 도구 사용과 상호보완적이다.

**[[LLM Agent]]** 엔티티와도 관련이 깊다. LLM 기반 에이전트에서 경험 재사용과 스킬 라이브러리 구축은 AgentFactory의 자기 진화 프레임워크, Android Coach의 온라인 에이전트 학습과 같은 맥락에 있다.

### 핵심 기여

동적 스킬 뱅크는 정적 스킬 저장소와 달리 정책과 함께 공동 학습(jointly train)되어 지속적으로 진화한다. 이는 ChameleonEpisodicMemory의 에피소딕 메모리 관리나 CoupledControlStructuredMemory의 구조화된 메모리 접근과 유사한 **동적 메모리 관리** 패러다임에 속한다.

## 🔗 관련 논문

- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- Android Coach: Improve Online Agentic Training Effi
- AgentFactory: A Self-Evolving Framework Through Executable S
- Robust Quadruped Locomotion via Evolutionary Reinf

## 🏷️ 엔티티

- [[entities/llm-agent.md|LLM Agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
