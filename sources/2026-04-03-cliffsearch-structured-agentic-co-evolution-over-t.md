# CliffSearch: Structured Agentic Co-Evolution over Theory and Code for Scientific Algorithm Discovery

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.01210v1

## 💡 핵심 인사이트

과학적 알고리즘 발견에서 코드만 최적화하는 기존 접근의 한계를 극복하기 위해, 이론적 가설과 코드 구현을 LLM 에이전트 기반 진화 루프에서 함께 공진화시키는 구조가 효과적이다.

## 📖 분석

## CliffSearch: Structured Agentic Co-Evolution over Theory and Code for Scientific Algorithm Discovery

**CliffSearch**는 과학적 알고리즘 발견을 위한 에이전틱 진화 프레임워크로, LLM 에이전트가 진화 연산자(쌍 선택, 교차, 돌연변이, 리뷰)를 수행하며 이론과 코드를 공진화(co-evolution)시키는 구조를 제안한다.

### 핵심 문제의식
기존 LLM 기반 탐색 시스템들은 제안 생성을 가속화하지만, 코드 전용 아티팩트만 최적화하며 과학적 구조를 충분히 반영하지 못한다. 정확성(correctness)과 독창성(originality) 게이팅이 약하다는 한계가 있다. CliffSearch는 이론적 가설과 코드 구현을 분리하지 않고 함께 진화시킴으로써, 과학적 발견 과정의 반복적 특성(가설 제안 → 구현 → 스트레스 테스트 → 수정)을 충실히 모델링한다.

### 기존 연구와의 연결
- **[[concepts/autoresearch.md|autoresearch]]**: Bilevel Autoresearch가 메타 수준에서 연구 자동화를 다뤘다면, CliffSearch는 알고리즘 발견이라는 구체적 도메인에서 이론-코드 공진화라는 구조화된 접근을 취한다. 두 연구 모두 LLM을 연구 자동화의 핵심 엔진으로 활용하는 점에서 궤를 같이한다.
- **[[concepts/code-generation.md|code generation]]**: AVO(Agentic Variation Operators)가 진화적 코드 생성에 에이전트를 활용했다면, CliffSearch는 코드뿐 아니라 이론적 가설까지 진화 대상에 포함시킨 점이 차별적이다.
- **[[concepts/multi-agent-system.md|multi agent system]]**: 진화 연산자 각각을 독립 LLM 에이전트로 구현한 설계는 다중 에이전트 시스템의 역할 분화 패러다임과 일치한다.
- **[[entities/llm-agent.md|llm agent]]**: 구조화된 에이전틱 루프 설계로, 단순 프롬프트 체이닝을 넘어 과학적 방법론을 에이전트 워크플로우에 내재화한 사례다.

### 의의
이론과 코드의 공진화라는 프레임은 LLM 기반 과학 연구 자동화에서 '구현만 최적화하는' 함정을 피하는 중요한 설계 원칙을 제시한다.

## 🔗 관련 논문

- Bilevel Autoresearch: Meta-Autoresearching Itself
- AVO: Agentic Variation Operators for Autonomous Evolutionary
- Paper Circle: An Open Source Multi-Agent Research D
- AgentFactory: A Self-Evolving Framework Through Executable S

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/autoresearch.md|autoresearch]]
- [[concepts/code-generation.md|code-generation]]
- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/metaheuristic-optimization.md|metaheuristic-optimization]]

---
_LLM 분석으로 재생성됨_
