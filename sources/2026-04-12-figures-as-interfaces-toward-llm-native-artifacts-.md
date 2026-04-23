# Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-12
**링크**: http://arxiv.org/abs/2604.08491v1

## 💡 핵심 인사이트

과학적 figure를 정적 이미지가 아닌 LLM이 직접 조작 가능한 구조화된 인터페이스(LLM-native artifact)로 재설계함으로써, human-AI 과학 협업의 반복적 탐색과 재현성을 근본적으로 향상시킬 수 있다.

## 📖 분석

## Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

본 논문은 과학적 워크플로우에서 LLM이 생성하는 figure(그림/차트)를 단순한 정적 시각 요약이 아닌, LLM이 직접 조작·추론·재활용할 수 있는 **인터페이스**로 재정의할 것을 제안한다. 기존 패러다임에서 figure는 렌더링 후 픽셀이나 캡션으로 재해석되는 최종 산출물이었으나, LLM의 도구 사용(tool-use), 데이터 추론, 복잡한 분석 태스크 조율 능력이 발전하면서 figure 자체를 구조화된 데이터 객체(LLM-native artifact)로 설계할 수 있다는 관점이다.

### 기존 Wiki와의 관계

- **[[concepts/ai-artifact-design.md|ai artifact design]]**: 이 논문은 기존 ai-artifact-design 개념의 핵심 소스로, LLM 네이티브 아티팩트의 구체적 설계 원칙을 제시한다.
- **[[concepts/multimodal-llm.md|multimodal llm]]**: 멀티모달 LLM이 figure를 이미지로 재해석하는 현재 한계를 지적하며, 텍스트-구조 기반 대안을 제안한다.
- **[[concepts/tool-use.md|tool use]]**: LLM의 도구 사용 능력을 figure 생성·조작에 확장 적용하는 프레임워크를 논의한다.
- **[[concepts/shared-state-architecture.md|shared state architecture]]** / **[[concepts/context-bus.md|context bus]]**: figure를 공유 상태 객체로 다루는 접근은 PSI 논문의 shared-state 아키텍처와 개념적으로 연결된다.

### 핵심 기여

1. Figure를 정적 이미지가 아닌 **구조화된 인터페이스**로 재개념화
2. LLM이 figure의 데이터·레이아웃·의미를 직접 접근·수정할 수 있는 아키텍처 제안
3. 과학적 발견 워크플로우에서 human-AI 협업의 새로운 상호작용 패턴 탐구

## 🔗 관련 논문

- 2026 04 11 figures as interfaces toward llm native artifacts
- 2026 04 11 psi shared state as the missing layer for coherent
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/ai-artifact-design.md|ai-artifact-design]]
- [[concepts/multimodal-llm.md|multimodal-llm]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/shared-state-architecture.md|shared-state-architecture]]

---
_LLM 분석으로 생성됨_
