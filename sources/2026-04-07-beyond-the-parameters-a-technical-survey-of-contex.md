# Beyond the Parameters: A Technical Survey of Contextual Enrichment in Large Language Models: From In-Context Prompting to Causal Retrieval-Augmented Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-07
**링크**: http://arxiv.org/abs/2604.03174v1

## 💡 핵심 인사이트

LLM 컨텍스트 보강 전략을 '비구조적→구조적→인과적' 연속체로 통합하며, CausalRAG가 기존 RAG의 허위상관 문제를 인과 그래프로 해결하는 차세대 패러다임으로 부상하고 있다.

## 📖 분석

## Beyond the Parameters: Contextual Enrichment in LLMs 기술 서베이

본 서베이는 LLM의 정적 파라미터 한계를 극복하기 위한 **컨텍스트 보강 전략**을 단일 축(추론 시 제공되는 구조화된 컨텍스트의 정도)으로 통합 정리한다. In-Context Learning(ICL), Prompt Engineering, RAG, GraphRAG, 그리고 새롭게 부상하는 **CausalRAG**까지를 포괄적으로 다룬다.

### 핵심 프레임워크

논문은 컨텍스트 보강을 **비구조적→구조적→인과적** 스펙트럼으로 배치한다:
- **ICL/Prompt Engineering**: 최소 구조, 프롬프트 내 예시로 행동 유도
- **RAG**: 외부 문서 검색을 통한 지식 주입, 정적 파라미터의 한계 보완
- **GraphRAG**: 지식 그래프 기반 구조화된 검색으로 관계 추론 강화
- **CausalRAG**: 인과 관계를 명시적으로 모델링하여 검색된 컨텍스트의 추론 품질 향상

### 기존 Wiki와의 연결

이 서베이는 기존 Wiki의 여러 핵심 개념을 관통한다. [[concepts/retrieval-augmented-generation.md|retrieval augmented generation]]과 직접적으로 연결되며, RAG의 한계와 발전 방향을 체계적으로 정리한다. [[concepts/prompt-engineering.md|prompt engineering]]의 ICL 측면을 이론적으로 재조명하고, [[concepts/reasoning-chain.md|reasoning chain]] 및 [[concepts/reasoning-integrity.md|reasoning integrity]]와 관련하여 인과적 추론의 중요성을 강조한다. 또한 [[concepts/knowledge-injection.md|knowledge injection]]의 다양한 방법론을 통합적 관점에서 비교하며, [[concepts/process-control-architecture.md|process control architecture]]와 유사하게 LLM 추론 파이프라인의 구조화를 논의한다.

CausalRAG는 기존 RAG가 단순 유사도 기반 검색에 머무는 한계를 지적하며, 인과 그래프를 활용한 검색이 허위상관(spurious correlation) 문제를 완화할 수 있음을 제시한다. 이는 [[concepts/mechanistic-interpretability.md|mechanistic interpretability]]의 인과적 분석 방법론과도 맥을 같이 한다.

## 🔗 관련 논문

- Evaluating Chunking Strategies For Retrieval-Augmented Gener
- SPA: A Simple but Tough-to-Beat Baseline for Kno
- Box Maze: A Process-Control Architecture for Reliable LLM Re
- A Creative Agent is Worth a 64-Token Template
- MARCH: Multi-Agent Reinforced S
- Cram Less to Fit More: Training Data Pruning Improves Memori
- What Drives Representation Steering? A Mechanistic Case Stud

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[concepts/prompt-engineering.md|prompt-engineering]]
- [[concepts/knowledge-injection.md|knowledge-injection]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/causal-rag.md|causal-rag]]
- [[concepts/graph-rag.md|graph-rag]]
- [[concepts/in-context-learning.md|in-context-learning]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[entities/retrieval-augmented-generation.md|retrieval augmented generation]]

---
**관련**: [[entities/robotics-foundation-model.md|robotics foundation model]]

---
**관련**: [[concepts/process-reward-model.md|process reward model]]

---
**관련**: [[concepts/natural-language-symbolic-duality.md|natural language symbolic duality]]

---
**관련**: [[concepts/mixture-model.md|mixture model]]

---
**관련**: [[concepts/image-generation.md|image generation]]

---
**관련**: [[concepts/natural-language-to-formal-language.md|natural language to formal language]]

---
**관련**: [[concepts/language-agnostic-function-vector.md|language agnostic function vector]]

---
**관련**: [[concepts/layout-to-image-generation.md|layout to image generation]]

---
**관련**: [[concepts/ai-augmented-ecosystem.md|ai augmented ecosystem]]

---
**관련**: [[concepts/generative-model-planning.md|generative model planning]]

---
**관련**: [[concepts/user-turn-generation.md|user turn generation]]

---
**관련**: [[concepts/model-independent-safety-defect.md|model independent safety defect]]

---
**관련**: [[concepts/autoregressive-generation.md|autoregressive generation]]

---
**관련**: [[concepts/3d-generation.md|3d generation]]

---
**관련**: [[concepts/hardware-roofline-model.md|hardware roofline model]]

---
**관련**: [[concepts/dynamic-context-injection.md|dynamic context injection]]

---
**관련**: [[concepts/context-assemble-bridge.md|context assemble bridge]]

---
**관련**: [[concepts/in-context-grammar-interpretation.md|in context grammar interpretation]]

---
**관련**: [[concepts/reflective-context-learning.md|reflective context learning]]

---
**관련**: [[concepts/synchronous-context-free-grammar.md|synchronous context free grammar]]

---
**관련**: [[concepts/visual-workflow-generation.md|visual workflow generation]]

---
**관련**: [[concepts/natural-language-to-executable-pipeline.md|natural language to executable pipeline]]

---
**관련**: [[concepts/context-space-optimization.md|context space optimization]]

---
**관련**: [[entities/adversarial-problem-generation.md|adversarial problem generation]]

---
**관련**: [[entities/draft-model-domain-adaptation.md|draft model domain adaptation]]

---
**관련**: [[entities/model-context-protocol.md|model context protocol]]

---
**관련**: [[entities/diffusion-model.md|diffusion model]]

---
**관련**: [[entities/model-organism.md|model organism]]

---
**관련**: [[entities/class-level-code-generation.md|class level code generation]]

---
**관련**: [[concepts/behavior-infrastructure-dual-cost-model.md|behavior infrastructure dual cost model]]

---
**관련**: [[concepts/context-fracture-point.md|context fracture point]]

---
**관련**: [[concepts/annotation-model-conflation.md|annotation model conflation]]

---
**관련**: [[concepts/context-as-pipeline-structural-constraint.md|context as pipeline structural constraint]]

---
**관련**: [[concepts/bidirectional-context-modeling.md|bidirectional context modeling]]

---
**관련**: [[concepts/retry-context-accumulation-loop.md|retry context accumulation loop]]

---
**관련**: [[concepts/tool-context-optimization.md|tool context optimization]]

---
**관련**: [[concepts/video-game-generation.md|video game generation]]

---
**관련**: [[concepts/draft-model-domain-adaptation.md|draft model domain adaptation]]

---
**관련**: [[concepts/causal-mechanistic-interpretability.md|causal mechanistic interpretability]]

---
**관련**: [[concepts/authority-model-of-annotation.md|authority model of annotation]]

---
**관련**: [[concepts/evidence-model-of-annotation.md|evidence model of annotation]]

---
**관련**: [[concepts/reproducible-specification-generation.md|reproducible specification generation]]

---
**관련**: [[concepts/extension-model-of-annotation.md|extension model of annotation]]

---
**관련**: [[concepts/adversarial-problem-generation.md|adversarial problem generation]]
