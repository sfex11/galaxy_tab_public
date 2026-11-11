# Contrastive Discovery: Open-Ended Scientific Discovery over Competing Explanations

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14514v1

## 💡 핵심 인사이트

가설을 보집합(¬h)과 비교하는 점별 검증은 증거의 정보량을 구조적으로 제한하므로, 상호 배타적 대조 집합으로 가설 공간을 먼저 재구성하는 것이 실험 효율의 선행 조건이다.

## 📖 분석

## Contrastive Discovery: Open-Ended Scientific Discovery over Competing Explanations (2026-11-12)

데이터 기반 개방형 과학 발견 에이전트가 가설 h를 보집합 ¬h와만 비교하는 점별(pointwise) 검증에 의존한다는 진단에서 출발한다. 이 구조에서 증거가 h를 기각해도 에이전트는 '한 설명이 기각되었다'만 배울 뿐 어느 대안이 지지되는지 알 수 없다. 본 논문은 과학 질문과 상호 배타적 후보 설명들로 구성된 대조 집합(contrast set)을 도입해, 실험이 설명들 사이를 식별하도록 만든다.

가설 탐색 메커니즘 계보에서 위치가 명확하다. HypoEvolve([[evolutionary-hypothesis-search]])가 유전적 변이·도태를, Night Scientist([[ai-night-scientist]])가 RL 이데이션을 제공했다면, 본 논문은 가설 공간의 평가 구조 자체를 설계 대상으로 삼는 제3 경로다. [[unguided-scientific-discovery]](자유 탐색 물리 법칙 발견)가 관찰→가설→실험→법칙 전 루프를 평가했다면, 본 논문은 그 루프 내 가설-증거 인터페이스의 정보 병목을 국소화한다.

[[expected-value-of-information]] 관점에서 상호 배타적 대조 집합은 실험의 판별력과 정보 획득을 증폭시키며, [[prior-weighted-bisection]]과 [[question-generation-as-belief-modeling]]이 확립한 '가설 공간 분할 질문' 패러다임의 과학 발견 도메인 실현이다. [[failed-hypothesis-tracking]]이 실패 사후 추적으로 대안을 복원했다면, 대조 집합은 대안을 실험 전에 외현화한다.

## 🔗 관련 논문

- HypoEvolve: Genetic Algorithms Enable Multi-Agent LLMs to Discover Scientific Hypotheses
- Can LLMs Uncover Hidden Physical Laws through Free Exploration?
- Reinforcing Agentic Creativity in Scientific Ideation with Night Scientist
- AI Co-Mathematician: Accelerating Mathematicians with Agentic AI
- Playing log(N)-Questions over Wikipedia Abstracts: Communication Efficiency of Language Model Collectives

## 🏷️ 엔티티

- [[entities/contrastive-discovery.md|contrastive-discovery]]
- [[entities/evolutionary-hypothesis-search.md|evolutionary-hypothesis-search]]
- [[entities/unguided-scientific-discovery.md|unguided-scientific-discovery]]

## 📐 개념

- [[concepts/contrast-set-hypothesis-testing.md|contrast-set-hypothesis-testing]]
- [[concepts/pointwise-complement-conflation.md|pointwise-complement-conflation]]
- [[concepts/expected-value-of-information.md|expected-value-of-information]]
- [[concepts/relative-verifiability.md|relative-verifiability]]
- [[concepts/extra-probabilistic-adjudication.md|extra-probabilistic-adjudication]]
- [[concepts/prior-weighted-bisection.md|prior-weighted-bisection]]
- [[concepts/question-generation-as-belief-modeling.md|question-generation-as-belief-modeling]]
- [[concepts/failed-hypothesis-tracking.md|failed-hypothesis-tracking]]
- [[concepts/hypothesis-selection-evaluation.md|hypothesis-selection-evaluation]]

---
_LLM 분석으로 생성됨_
