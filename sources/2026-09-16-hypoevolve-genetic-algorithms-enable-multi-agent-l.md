# HypoEvolve: Genetic Algorithms Enable Multi-Agent LLMs to Discover Scientific Hypotheses

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15938v1

## 💡 핵심 인사이트

다중 에이전트 과학 시스템에서 협력 구조는 모델 능력과 독립적으로 가설 품질을 결정하는 인과 변수이며, 이 둘을 분리하는 통제 실험 설계가 연구 자동화 시스템의 성숙도를 평가하는 새로운 방법론적 기준이 된다.

## 📖 분석

HypoEvolve는 유전 알고리즘의 진화 탐색을 다중 LLM 과학 에이전트(증거 종합, 제안 평가, 설명 개발)와 결합하여 가설 발견을 자동화한다. 핵심 질문은 '에이전트 협력 형태가 가설 품질에 어떤 영향을 주는가'이며, 이에 답하기 위해 과학적 능력(capability)과 협력 구조(collaboration)의 효과를 분리하는 실험 프레임워크를 제시한다.

이 분해 전략은 [[capability-cooperation-paradox]]의 진단적 보완이다 — 역설이 '능력이 협력을 저해한다'는 상관 관찰이었다면, 본 논문은 능력을 통제한 채 협력 위상만 변이시켜 협력 자체의 독립 효과를 검증하는 인과 분해로 나아간다. [[independent-effect-tracking-problem]]이 '방법론적으로 불가능'하다고 기술한 밀결합 시스템의 요소 기여 격리를 연구 에이전트 도메인에서 통제 실험으로 실현한 사례다.

진화 메커니즘은 [[cooperation-competition-spectrum]]의 하이브리드 실현이기도 하다 — 선택·도태는 경쟁적 압력, 비평·비교·수정은 협력적 정제로 작동하여 두 위상이 단계별로 공존한다. 가설을 진화 단위로 삼는 것은 [[evolutionary-agency-axis]]에서 외생적 진화의 과학 발견 버전이며, 적합도 함수 설계가 곧 '좋은 가설'의 정의를 결정하는 [[selection-pressure-design]] 문제로 이어진다.

## 🔗 관련 논문

- SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Interpretability Research
- Autonomous Research for Open-Ended Problems: A Case Study
- Avatar: Toward Autonomous End-to-End Orchestration of Scientific Workflows

## 🏷️ 엔티티

- [[entities/capability-collaboration-decoupling.md|capability-collaboration-decoupling]]
- [[entities/evolutionary-hypothesis-search.md|evolutionary-hypothesis-search]]
- [[entities/capability-cooperation-paradox.md|capability-cooperation-paradox]]
- [[entities/cooperation-competition-spectrum.md|cooperation-competition-spectrum]]
- [[entities/exploratory-research-agent.md|exploratory-research-agent]]
- [[entities/independent-effect-tracking-problem.md|independent-effect-tracking-problem]]
- [[entities/evolutionary-agency-axis.md|evolutionary-agency-axis]]
- [[entities/selection-pressure-design.md|selection-pressure-design]]
- [[entities/hypothesis-selection-evaluation.md|hypothesis-selection-evaluation]]
- [[entities/autoresearch.md|autoresearch]]

## 📐 개념

- [[concepts/capability-collaboration-decoupling.md|capability-collaboration-decoupling]]
- [[concepts/evolutionary-hypothesis-search.md|evolutionary-hypothesis-search]]

---
_LLM 분석으로 생성됨_
