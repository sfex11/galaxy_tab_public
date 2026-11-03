# From Natural Language to Exact Cover: A Neuro-Symbolic Approach to Zebra Puzzles

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03641v1

## 💡 핵심 인사이트

순수 신경망 추론의 결정론성·건전성 결여에 대해 LLM을 의미 번역기로, 정확 커버 솔버를 추론 엔진으로 분리하는 신경-기호 하이브리드가 신뢰성 병목을 '추론 능력'에서 '번역 충실도'로 이동시킨다.

## 📖 분석

본 논문은 CoT 기반 순수 신경망 추론이 논리 퍼즐(Zebra 퍼즐)에서 결정론성·건전성·신뢰성을 담보하지 못하는 한계를, 자연어→정확 커버(exact cover) 축소라는 신경-기호 하이브리드로 해결한다. LLM은 퍼즐 서술을 형식 인코딩으로 번역하는 의미 파서 역할을 수행하고, 정확 커버 솔버가 결정론적 해답을 산출한다.

이는 [[natural-language-to-formal-language]]의 진단(Syntax Is Easy, Semantics Is Hard)에 제3의 해법을 제공한다 — 번역과 추론을 계층 분리하여 각 계층에 적합한 엔진을 배치하는 것이다. 이 배치는 [[external-layer-principle]]의 구현 사례로서, 형식 추론의 검증 기준이 LLM 외부의 기호 체계에 귀속된다.

[[llm-falsifier]]가 LLM을 형식 오라클 피드백 하의 블랙박스 최적화기로 배치했다면, 본 논문은 역할을 반전시켜 LLM을 번역자로, 기호 엔진을 추론 주체로 삼는다. 두 사례의 대비는 신경-기호 결합에서 역할 배분이 설계 자유 변수임을 확정한다.

구조적 함의: 솔버의 건전성은 인코딩이 충실할 때만 유효하므로, 신뢰성 병목이 '추론 능력'에서 '번역 충실도'로 이동한다. 이는 [[representation-contract]]의 형식적 유효성(잘 구성된 인코딩)과 실질적 이행(의미 충실성)의 분리 원리를 논리 도메인에서 확정하며, [[verification-as-system-external-relation]]이 강조하는 검증 가능성의 시스템-외부성을 강화한다.

## 🔗 관련 논문

- Syntax Is Easy, Semantics Is Hard: Evaluating LLMs for LTL Translation
- Large Language Models as Falsifiers for Cyber-Physical Systems
- RunAgent: Interpreting Natural-Language Plans with Constraint-Guided Execution

## 🏷️ 엔티티

- [[entities/neuro-symbolic-division-of-labor.md|neuro-symbolic-division-of-labor]]
- [[entities/exact-cover-reduction.md|exact-cover-reduction]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/llm-falsifier.md|llm-falsifier]]
- [[entities/formal-verification.md|formal-verification]]

## 📐 개념

- [[concepts/encoding-faithfulness-bottleneck.md|encoding-faithfulness-bottleneck]]
- [[concepts/external-layer-principle.md|external-layer-principle]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[concepts/hybrid-verification-architecture.md|hybrid-verification-architecture]]
- [[concepts/constraint-guided-plan-execution.md|constraint-guided-plan-execution]]

---
_LLM 분석으로 생성됨_
