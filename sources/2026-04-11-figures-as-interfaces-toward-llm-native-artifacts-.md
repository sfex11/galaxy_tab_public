# Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-11
**링크**: http://arxiv.org/abs/2604.08491v1

## 💡 핵심 인사이트

과학적 시각화(figure)를 LLM이 직접 조작 가능한 구조화된 인터페이스로 재설계하면, 정적 이미지 재해석의 정보 손실 없이 인간-AI 과학 협업의 효율성을 근본적으로 높일 수 있다.

## 📖 분석

## Figures as Interfaces: Toward LLM-Native Artifacts for Scientific Discovery

본 논문은 과학적 워크플로우에서 LLM이 생성하는 시각화(figure)를 단순한 정적 이미지가 아닌, LLM이 직접 조작하고 추론할 수 있는 **인터페이스**로 재정의할 것을 제안한다. 기존 인간-AI 협업에서 figure는 렌더링 후 픽셀이나 캡션으로 재해석되는 정적 산출물에 불과했으나, LLM의 도구 사용(tool-use) 및 데이터 추론 능력이 발전하면서 figure 자체를 구조화된 상호작용 가능한 아티팩트로 설계할 수 있다는 비전을 제시한다.

### 기존 Wiki와의 관계

- **tool-use**: 본 논문의 핵심 전제는 LLM의 도구 사용 능력이다. LLM이 figure를 생성할 뿐 아니라 figure의 구조화된 데이터를 도구로 활용하여 분석 파이프라인을 조율하는 패러다임을 논한다.
- **LLM Agent**: figure를 인터페이스로 활용하는 LLM은 본질적으로 에이전트적(agentic) 행동을 수행한다. 복잡한 분석 태스크를 조율하고 데이터에 대해 추론하는 능력이 LLM Agent 개념과 직접 연결된다.
- **multimodal-learning / multimodal-llm**: 멀티모달 LLM이 이미지를 픽셀 단위로 재해석하는 현재 방식의 한계를 지적하며, 구조화된 표현이 더 효과적임을 주장한다.

### 새로운 관점

이 논문은 LLM의 출력물 형식(artifact format) 자체를 재설계해야 한다는 메타 수준의 제안으로, 기존 Wiki의 도구 사용이나 에이전트 연구가 주로 입력/프로세스에 초점을 맞춘 것과 달리 **출력 아티팩트의 구조**에 주목한다는 점에서 차별화된다.

## 🔗 관련 논문

- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 how much llm does a self revising agent actually n
- 2026 04 09 paper circle an open source multi agent research d

## 🏷️ 엔티티

- [[entities/llm.md|LLM]]

## 📐 개념

- [[concepts/tool-use.md|tool-use]]
- [[concepts/multimodal-llm.md|multimodal-llm]]
- [[concepts/ai-artifact-design.md|ai-artifact-design]]

---
_LLM 분석으로 생성됨_
