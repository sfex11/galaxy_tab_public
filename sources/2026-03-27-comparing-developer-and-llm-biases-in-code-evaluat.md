# Comparing Developer and LLM Biases in Code Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-27
**링크**: http://arxiv.org/abs/2603.24586v1

## 💡 핵심 인사이트

LLM 심판과 인간 개발자는 코드 평가 시 체계적으로 다른 루브릭 항목에 가중치를 부여하며, TRACE 프레임워크를 통해 이러한 편향 차이를 정량적으로 식별할 수 있다.

## 📖 분석

## Comparing Developer and LLM Biases in Code Evaluation

본 논문은 LLM을 코드 평가의 심판(judge)으로 활용할 때 발생하는 체계적 편향을 인간 개발자의 편향과 비교 분석한다. 저자들은 TRACE(Tool for Rubric Analysis in Code Evaluation)라는 프레임워크를 제시하여, 채팅 기반 프로그래밍, IDE 자동완성, 지시 기반 코드 편집의 세 가지 모달리티에서 LLM 심판이 인간 선호를 예측하는 능력을 평가하고, 루브릭 항목별 가중치의 차이를 자동 추출한다.

### 핵심 기여
- **TRACE 프레임워크**: 코드 평가에서 인간과 LLM의 판단 기준을 루브릭 항목 단위로 분해하여 체계적 편향을 식별하는 도구
- **편향 비교 분석**: 개발자와 LLM이 코드 품질을 평가할 때 서로 다른 루브릭 항목에 가중치를 부여하는 패턴을 발견
- **현실적 평가 설정**: 부분적 컨텍스트와 모호한 의도가 존재하는 실제 인터랙티브 환경에서의 평가

### 기존 Wiki와의 연결
본 논문은 [[concepts/llm-benchmark.md|llm benchmark]] 개념과 직접 연결되며, LLM-as-Judge 패러다임의 신뢰성 문제를 다룬다는 점에서 [[concepts/reasoning-integrity.md|reasoning integrity]]와도 관련된다. [[concepts/code-generation.md|code generation]] 분야에서 생성된 코드의 평가 방법론을 제공하며, LLM 편향 분석이라는 측면에서 [[concepts/llm-alignment.md|llm alignment]] 및 [[concepts/adversarial-prompting.md|adversarial prompting]] 연구와도 접점이 있다. 특히 자동화된 판단의 신뢰성을 다루는 점에서 Evaluating the Reliability and Fidelity of Automated Judgments 논문과 상호보완적이다.

## 🔗 관련 논문

- 2026 03 25 evaluating the reliability and fidelity of automat
- 2026 04 10 chatbot based assessment of code understanding in
- 2026 03 22 box maze a process control architecture for reliab
- 2026 04 09 paper circle an open source multi agent research d

## 🏷️ 엔티티

- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/llm-benchmark.md|llm-benchmark]]
- [[concepts/reasoning-integrity.md|reasoning-integrity]]
- [[concepts/code-generation.md|code-generation]]
- [[concepts/llm-alignment.md|llm-alignment]]
- [[concepts/adversarial-prompting.md|adversarial-prompting]]

---
_LLM 분석으로 재생성됨_
