# MTI: A Behavior-Based Temperament Profiling System for AI Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02145v1

## 💡 핵심 인사이트

LLM의 자기보고와 실제 행동 간 괴리를 인식하고, 관찰 가능한 행동 패턴에서 직접 기질을 측정하는 표준화된 프로파일링 체계를 최초로 제안했다는 점에서, AI 에이전트 평가 패러다임을 '능력 측정'에서 '성향 측정'으로 확장한다.

## 📖 분석

## MTI: AI 에이전트를 위한 행동 기반 기질 프로파일링 시스템

### 핵심 내용
Model Temperament Index(MTI)는 AI 에이전트의 **행동 기반 기질(temperament)**을 측정하는 표준화된 프로파일링 시스템이다. 기존 접근법들이 인간 성격 심리학의 차원을 차용하거나 자기보고(self-report) 방식에 의존한 반면, MTI는 LLM의 자기보고와 실제 행동 간 괴리를 인식하고 **관찰 가능한 행동 패턴**에서 직접 기질을 측정한다. 4개 차원에 걸쳐 에이전트 간 성향 차이를 정량화한다.

### 기존 연구와의 연결
이 연구는 LLM 에이전트의 내부 작동을 이해하려는 **mechanistic interpretability** 흐름과 맞닿아 있으며, 특히 [[concepts/representation-steering.md|representation steering]] 연구에서 모델 행동을 조향할 때 기질 프로파일이 사전 진단 도구로 활용될 수 있다. [[concepts/ai-governance.md|ai governance]] 및 [[concepts/ai-safety.md|ai safety]] 관점에서는 에이전트 배포 전 행동 성향을 평가하는 프레임워크로서 [[The Stochastic Gap]]의 사전 배포 신뢰성 평가와 상호 보완적이다. [[concepts/cognitive-architecture.md|cognitive architecture]]의 Triadic Cognitive Architecture가 에이전트 자율성의 경계를 설정한다면, MTI는 그 경계 내에서 에이전트가 어떤 **행동 양식**을 보이는지를 프로파일링한다. 또한 [[concepts/choice-architecture.md|choice architecture]]의 Mecha-nudges 연구와 연결되는데, 에이전트의 기질을 알면 넛지 설계를 더 정밀하게 할 수 있다. LLM 자기보고의 한계를 지적한다는 점에서 [[concepts/llm-benchmark.md|llm benchmark]] 평가 방법론에 대한 비판적 시사점도 있다.

## 🔗 관련 논문

- 2026-03-27 the stochastic gap a markovian framework for pre d
- 2026-04-02 the triadic cognitive architecture bounding autono
- 2026-04-11 what drives representation steering a mechanistic 
- 2026-03-26 mecha nudges for machines
- 2026-04-11 act wisely cultivating meta cognitive tool use in 
- 2026-03-26 beyond preset identities how agents form stances a

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/ai-agent-profiling.md|ai-agent-profiling]]
- [[concepts/behavioral-temperament.md|behavioral-temperament]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/ai-governance.md|ai-governance]]
- [[concepts/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[concepts/cognitive-architecture.md|cognitive-architecture]]
- [[concepts/choice-architecture.md|choice-architecture]]

---
_LLM 분석으로 재생성됨_
