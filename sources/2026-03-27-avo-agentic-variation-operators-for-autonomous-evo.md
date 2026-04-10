# AVO: Agentic Variation Operators for Autonomous Evolutionary Search

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24517v1

## 💡 핵심 인사이트

AVO는 LLM 에이전트를 진화 알고리즘의 변이 연산자로 활용함으로써, 고정된 휴리스틱 기반 탐색을 자율적 코드 생성·수정·비판 루프로 대체하는 새로운 패러다임을 제시한다.

## 📖 분석

## AVO: Agentic Variation Operators for Autonomous Evolutionary Search

**Agentic Variation Operators(AVO)**는 고전적 진화 탐색의 고정된 변이(mutation), 교차(crossover), 수작업 휴리스틱을 자율 코딩 에이전트로 대체하는 새로운 진화적 변이 연산자 패밀리다. 기존 진화 알고리즘이 사전 정의된 파이프라인 내에서 후보를 생성하는 데 그쳤다면, AVO는 변이 자체를 자기 주도적 에이전트 루프로 인스턴스화한다. 이 에이전트는 현재 계보(lineage), 도메인 특화 지식 베이스, 실행 피드백을 참조하여 후보 솔루션을 제안·수정·비판·개선할 수 있다.

### 핵심 기여
- **에이전트 기반 변이**: LLM 에이전트가 진화 연산자 역할을 수행하며, 단순 프롬프트 기반 생성을 넘어 자율적 탐색·수정·자기비판 루프를 구현
- **지식 베이스 통합**: 도메인 지식과 실행 피드백을 활용한 적응적 변이로, 기존 블라인드 탐색 대비 탐색 효율성 향상
- **자기 주도적 루프**: 에이전트가 계보 정보를 추적하며 점진적 개선을 자율 수행

### 기존 연구와의 연결
AVO는 **LLM Agent** 패러다임의 진화 알고리즘 적용 사례로, 에이전트가 도구를 사용하고 자기 피드백을 반영하는 구조는 [[ActWisely]]의 메타인지적 도구 사용 연구와 맥을 같이한다. 또한 자동화된 연구 파이프라인 관점에서 [[Bilevel Autoresearch]]의 메타-자동연구 프레임워크와 유사한 자기 참조적 최적화 구조를 공유한다. 코드 생성 및 수정 에이전트로서의 측면은 [[AgentFactory]]의 자기 진화 프레임워크와도 연결된다. 진화 탐색에 강화학습적 피드백 루프를 결합한 점에서 **Reinforcement Learning** 엔티티의 확장적 응용으로도 볼 수 있다.

## 🔗 관련 논문

- 2026 04 11 act wisely cultivating meta cognitive tool use in
- 2026 03 26 bilevel autoresearch meta autoresearching itself

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/metacognition.md|metacognition]]
- [[concepts/autoresearch.md|autoresearch]]
- [[concepts/code-generation.md|code-generation]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/prompt-engineering.md|prompt-engineering]]

---
_LLM 분석으로 재생성됨_
