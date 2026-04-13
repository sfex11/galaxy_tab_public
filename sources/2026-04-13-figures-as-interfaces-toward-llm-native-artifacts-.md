# Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-13
**링크**: http://arxiv.org/abs/2604.08491v1

## 💡 핵심 인사이트

과학 figure를 정적 이미지가 아닌 코드·데이터·메타데이터가 결합된 LLM-네이티브 아티팩트로 재정의하면, LLM이 픽셀 재해석 없이 직접 조작·추론할 수 있어 과학적 발견의 재현성과 인간-AI 협업 효율이 근본적으로 향상된다.

## 📖 분석

## Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

본 논문은 과학 워크플로우에서 LLM이 생성하는 figure를 정적 이미지가 아닌 **LLM-네이티브 인터페이스**로 재정의할 것을 제안한다. 기존 figure는 렌더링 후 픽셀/캡션 기반으로 재해석되지만, 저자들은 figure가 구조화된 데이터·코드·메타데이터를 포함하는 상호작용 가능한 아티팩트(artifact)가 되어야 한다고 주장한다.

### 기존 Wiki와의 관계
- **ai-artifact-design**: 본 논문의 핵심 주제. LLM이 과학적 발견을 위해 생성하는 아티팩트의 설계 패러다임을 정의한다.
- **shared-state-architecture / context-bus**: PSI 논문과 유사하게, figure를 인간-AI 간 공유 상태(shared state)로 활용하는 구조를 제안한다. figure 내부의 구조화된 표현이 컨텍스트 버스 역할을 수행한다.
- **multimodal-llm**: 멀티모달 LLM이 이미지를 픽셀로 재해석하는 비효율성을 지적하며, 구조화된 표현을 통한 직접 접근을 대안으로 제시한다.
- **tool-use**: LLM의 도구 사용 능력(tool use)이 figure 생성·수정·분석의 전 과정에 활용되는 구조를 설명한다.

### 핵심 제안
Figure = 코드 + 데이터 + 메타데이터의 번들로, LLM이 직접 조작·추론·재생성할 수 있는 프로그래밍 가능한 객체. 이는 과학적 재현성과 인간-AI 협업 효율성을 동시에 높인다.

### 다른 논문과의 연결
- **PSI (Shared State)**: figure를 공유 상태 레이어로 보는 관점이 PSI의 아키텍처 철학과 직접 연결됨
- **SAGAI-MID**: 동적 런타임 미들웨어와 figure-as-interface의 상호운용성 가능성

## 🔗 관련 논문

- 2026 04 11 figures as interfaces toward llm native artifacts
- 2026 04 12 figures as interfaces toward llm native artifacts
- 2026 04 11 psi shared state as the missing layer for coherent
- 2026 04 12 psi shared state as the missing layer for coherent

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/ai-artifact-design.md|ai-artifact-design]]
- [[concepts/multimodal-llm.md|multimodal-llm]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/shared-state-architecture.md|shared-state-architecture]]
- [[concepts/context-bus.md|context-bus]]

---
_LLM 분석으로 생성됨_
