# Paper Circle: An Open-source Multi-agent Research Discovery and Analysis Framework

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-09
**링크**: http://arxiv.org/abs/2604.06170v1

## 💡 핵심 인사이트

Paper Circle은 멀티에이전트 LLM 시스템을 학술 연구 탐색에 적용하여, 검색-평가-합성의 전 과정을 역할 분화된 에이전트 협업으로 자동화한 오픈소스 프레임워크이다.

## 📖 분석

## Paper Circle: 오픈소스 멀티에이전트 연구 탐색 및 분석 프레임워크

Paper Circle은 과학 문헌의 폭발적 증가에 대응하여, 논문의 발견·평가·정리·이해에 필요한 노력을 줄이기 위해 설계된 멀티에이전트 연구 탐색 및 분석 시스템이다. 다수의 LLM 에이전트가 각각 특화된 역할(검색, 평가, 요약, 합성 등)을 수행하며, 도구 사용(tool-use) 능력을 활용해 외부 학술 데이터베이스와 상호작용한다.

### 핵심 설계 원리
- **역할 분화된 멀티에이전트 구조**: 각 에이전트가 검색, 관련성 평가, 비판적 분석, 종합 등 연구 워크플로우의 개별 단계를 담당
- **도구 활용(Tool-Use)**: 에이전트들이 학술 검색 API, 인용 그래프 등 외부 도구를 자율적으로 호출
- **오픈소스 접근**: 재현성과 확장성을 위한 공개 프레임워크

### 기존 연구와의 연결
Paper Circle은 [[concepts/multi-agent-system.md|multi agent system]] 패러다임의 학술 연구 자동화 적용 사례로, Bilevel Autoresearch의 메타 연구 자동화와 맥락을 같이한다. 에이전트의 도구 사용 능력은 [[concepts/tool-use.md|tool use]] 개념과 직결되며, AgentFactory의 자기진화 프레임워크와도 에이전트 협업 측면에서 비교할 수 있다. 또한 RAG 기반 검색과 결합하여 [[concepts/retrieval-augmented-generation.md|retrieval augmented generation]] 파이프라인의 에이전트 확장으로 볼 수 있다. CliffSearch의 에이전트 기반 이론 탐색과도 자동화된 연구 탐색이라는 공통 목표를 공유한다.

## 🔗 관련 논문

- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 03 26 bilevel autoresearch meta autoresearching itself
- 2026 04 03 cliffsearch structured agentic co evolution over t
- 2026 04 10 a systematic study of retrieval pipeline design fo
- 2026 04 11 act wisely cultivating meta cognitive tool use in

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/multi-agent-system.md|multi-agent-system]]

## 📐 개념

- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/autoresearch.md|autoresearch]]
- [[concepts/agent-coordination.md|agent-coordination]]

---
_LLM 분석으로 재생성됨_
