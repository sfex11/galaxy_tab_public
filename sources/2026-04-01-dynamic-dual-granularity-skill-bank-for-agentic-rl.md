# Dynamic Dual-Granularity Skill Bank for Agentic RL

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-01
**링크**: http://arxiv.org/abs/2603.28716v1

## 💡 핵심 인사이트

에이전틱 RL에서 태스크 수준과 스텝 수준의 이중 세분화 스킬 뱅크를 동적으로 유지함으로써, 경험 재사용의 세밀도와 적응성을 동시에 확보한다.

## 📖 분석

## Dynamic Dual-Granularity Skill Bank for Agentic RL (D2Skill)

**arXiv**: http://arxiv.org/abs/2603.28716v1
**날짜**: 2026-04-01

### 개요

D2Skill은 에이전틱 강화학습(Agentic RL)에서 재사용 가능한 경험을 **이중 세분화(dual-granularity) 스킬 뱅크**로 체계화하는 프레임워크다. 기존 스킬 기반 방법들이 주로 궤적(trajectory) 수준의 가이던스만 추출하고, 진화하는 스킬 메모리를 유지하는 원칙적 메커니즘이 부족했던 문제를 해결한다.

### 핵심 구조

- **Task Skills**: 높은 수준의 전략적 가이던스를 제공하는 태스크 단위 스킬
- **Step Skills**: 세밀한 의사결정 지원과 오류 수정을 위한 스텝 단위 스킬
- 정책(policy)과 스킬 뱅크를 **공동 학습(jointly train)**하여, 에이전트가 경험을 축적하면서 스킬 라이브러리를 동적으로 갱신

### 기존 연구와의 연결

이 연구는 [[reinforcement-learning]]의 에이전틱 확장으로, LLM Agent가 환경과 상호작용하며 스킬을 축적하는 패러다임을 제시한다. [[llm-agent]] 연구에서 도구 사용(tool-use)과 메타인지(metacognition) 능력이 강조되어 왔는데, D2Skill의 이중 세분화 접근은 [[metacognition]]의 '언제 어떤 스킬을 적용할지 판단'하는 메타 수준 의사결정과 직접 연결된다. 또한 [[hierarchical-representation]]의 다층적 추상화 개념을 스킬 관리에 적용한 것으로 볼 수 있다.

스킬 뱅크의 동적 갱신 메커니즘은 [[transfer-learning]]과 [[meta-learning]]에서 다뤄온 경험 재사용 문제의 실용적 해법이며, Android Coach의 온라인 에이전틱 학습 효율화 연구와도 상호 보완적이다.

## 🔗 관련 논문

- 2026 04 10 android coach improve online agentic training effi
- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 04 10 robust quadruped locomotion via evolutionary reinf

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/hierarchical-representation.md|hierarchical-representation]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/transfer-learning.md|transfer-learning]]
- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/tool-use.md|tool-use]]

---
_LLM 분석으로 재생성됨_
