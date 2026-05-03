# The Triadic Cognitive Architecture: Bounding Autonomous Action via Spatio-Temporal and Epistemic Friction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.30031v1

## 💡 핵심 인사이트

LLM 에이전트의 실패 모드를 '인지적 무중력' 문제로 재정의하고, 공간-시간적·인식론적 마찰을 아키텍처 수준에서 부과함으로써 휴리스틱 에이전트 루프의 구조적 취약성을 해결하는 새로운 프레임워크를 제시한다.

## 📖 분석

## The Triadic Cognitive Architecture

현재 LLM 기반 자율 에이전트가 겪는 근본적 문제를 '인지적 무중력(cognitive weightlessness)'으로 정의한 논문이다. 에이전트가 네트워크 토폴로지, 시간적 페이싱, 인식론적 한계에 대한 내재적 감각 없이 작동하면서 ReAct 등 휴리스틱 에이전트 루프에서 과도한 도구 사용, 시간 감쇠 하 지연된 숙고, 모호한 증거 하 취약한 행동 등의 실패 모드가 발생한다고 분석한다.

이를 해결하기 위해 **공간-시간적 마찰(spatio-temporal friction)**과 **인식론적 마찰(epistemic friction)**이라는 두 축의 제약을 부과하는 삼원 인지 아키텍처(Triadic Cognitive Architecture)를 제안한다. 이는 에이전트의 자율적 행동 범위를 명시적으로 경계짓는 구조적 접근이다.

### 기존 연구와의 관계

[[concepts/process-control-architecture.md|process control architecture]]의 Box Maze가 LLM 추론의 신뢰성을 프로세스 제어로 확보하려 했다면, 본 논문은 에이전트의 **행동 자체**에 마찰을 부여하는 더 포괄적 프레임워크를 제시한다. [[concepts/metacognition.md|metacognition]] 관점에서 Act Wisely의 메타인지적 도구 사용과도 맞닿아 있으며, [[concepts/tool-use.md|tool use]]의 과도한 호출 문제를 구조적으로 억제하는 메커니즘을 제공한다. [[concepts/ai-safety.md|ai safety]]의 TraceSafe가 가드레일 평가에 집중했다면, 본 연구는 가드레일이 필요해지기 전 단계에서 에이전트 행동을 제한하는 아키텍처 수준의 해법을 탐구한다.

## 🔗 관련 논문

- Box Maze: A Process-Control Architecture for Reliable LLM Re
- Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic M
- TraceSafe: A Systematic Assessment of LLM Guardrails on Mult
- PSI: Shared State as the Missing Layer for Coherent AI-Gener

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]

## 📐 개념

- [[concepts/cognitive-architecture.md|cognitive-architecture]]
- [[concepts/epistemic-friction.md|epistemic-friction]]
- [[concepts/tool-use.md|tool-use]]
- [[concepts/metacognition.md|metacognition]]
- [[concepts/process-control-architecture.md|process-control-architecture]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/epistemic-orientation.md|epistemic orientation]]
