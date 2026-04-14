# PSI: Shared State as the Missing Layer for Coherent AI-Generated Instruments in Personal AI Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08529v1

## 💡 핵심 인사이트

AI가 생성한 개별 모듈들의 고립 문제를 해결하기 위해, 공유 상태 레이어(shared-state layer)를 도입하여 독립적으로 생성된 모듈들을 일관된 도구 생태계로 통합할 수 있다.

## 📖 분석

## PSI: Shared State as the Missing Layer for Coherent AI-Generated Instruments in Personal AI Agents

PSI는 자연어 요청으로 생성된 개별 AI 모듈들을 **공유 상태(shared state)** 아키텍처를 통해 일관된 도구(instrument)로 통합하는 프레임워크다. 생성된 모듈이 생성 후 고립되는 문제를 해결하기 위해, 각 모듈이 현재 상태와 write-back affordance를 **개인 컨텍스트 버스(personal-context bus)**에 발행하여 모듈 간 추론과 동기화된 액션을 가능하게 한다.

### 기존 연구와의 관계

이 논문은 기존 Wiki의 [[shared-state-architecture]], [[context-bus]], [[personal-ai-agent]] 개념을 직접 확장한다. 2026-04-11 버전의 PSI 논문이 이미 Wiki에 등록되어 있으며(v1), 본 논문은 동일 연구의 최신 버전으로 아키텍처의 구체적 구현과 평가를 보강한다.

[[llm-middleware]] 개념과도 밀접하게 연결되는데, SAGAI-MID가 런타임 미들웨어를 통한 동적 연결을 다뤘다면, PSI는 **상태 공유**라는 더 근본적인 레이어에서 모듈 간 일관성을 보장한다. [[ai-artifact-design]]의 'Figures as Interfaces' 논문이 LLM 네이티브 아티팩트의 인터페이스 설계를 다뤘다면, PSI는 이러한 아티팩트들이 서로 **연결되어 작동하는 메커니즘**을 제시한다.

### 핵심 기여

- GUI와 채팅 에이전트 양쪽에서 접근 가능한 persistent instrument 개념 도입
- 모듈 간 cross-module reasoning을 위한 공유 상태 프로토콜 설계
- 생성형 AI 도구의 고립 문제(isolation problem)에 대한 구조적 해법 제시

[[schema-interoperability]]와도 관련되며, 모듈 간 상태 공유를 위한 스키마 설계가 상호운용성의 핵심 과제임을 보여준다.

## 🔗 관련 논문

- 2026 04 11 psi shared state as the missing layer for coherent
- 2026 04 12 psi shared state as the missing layer for coherent
- 2026 04 11 figures as interfaces toward llm native artifacts
- 2026 04 12 figures as interfaces toward llm native artifacts

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/shared-state-architecture.md|shared-state-architecture]]
- [[concepts/context-bus.md|context-bus]]
- [[concepts/personal-ai-agent.md|personal-ai-agent]]
- [[concepts/ai-artifact-design.md|ai-artifact-design]]
- [[concepts/llm-middleware.md|llm-middleware]]
- [[concepts/schema-interoperability.md|schema-interoperability]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-12-psi-shared-state-as-the-missing-layer-for-coherent]]: 동일 논문(PSI)의 다른 날짜 요약으로, AI 생성 모듈 간 공유 상태 레이어 아키텍처를 다룬다.
