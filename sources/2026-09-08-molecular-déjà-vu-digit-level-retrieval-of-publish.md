# Molecular Déjà Vu: Digit-Level Retrieval of Published Values in Frontier Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05381v1

## 💡 핵심 인사이트

분자 속성 벤치마크 정확도는 예측 능력과 기억된 수치 검색을 구별할 수 없으며, 자릿수 수준 감사 결과 verbatim 검색은 광범위하지만 벤치마크별로 이질적으로 분포한다.

## 📖 분석

# Molecular Déjà Vu: Digit-Level Retrieval of Published Values in Frontier Language Models (2026-09-08)

## 핵심 발견

LLM이 분자 속성 벤치마크에서 높은 정확도를 보여도, 그것이 속성의 '예측'인지 출판된 수치의 '검색'인지 구별할 수 없다. 22개 프론티어 모델을 12개 회귀 벤치마크에서 자릿수(digit) 수준 verbatim 검색으로 감사한 결과, 검색은 광범위하지만 벤치마크 특정적이다 — 5개 데이터셋에서 50% 이상의 모델이 verbatim 검색을 보이며, 나머지에서는 고립된 셀에서만 나타난다.

## Wiki 연결

[[fact-memorization]]에 문자열 수준을 넘어 자릿수 수준이라는 최대 엄격 기준의 실증을 제공한다. [[redirectqa]]와 [[entity-surface-form]] 계열 연구가 표면 형식을 다양화해 사실 기억과 접근성을 분리하려 했다면, 본 논문은 그 분리가 왜 필요한가에 대한 극단적 정당화 — 출판 값의 자릿수 재생 — 를 제시한다.

[[benchmark-specification-gap]] 관점에서 분자 벤치마크는 예측 능력과 검색 능력 중 무엇을 측정하는지 명세하지 않았으며, 정확도라는 [[meaning-insensitive-metric]]이 두 능력을 단일 점수로 병합하는 구조가 문제의 본질이다. [[data-contamination-resistance]]와 [[training-phase-knowledge-contamination]] 논의에 오염의 셀 수준 이질 분포라는 새로운 입자도를 부여한다.

## 새 개념

- **prediction-retrieval-ambiguity**: 벤치마크 정확도가 일반화된 예측과 기억된 검색을 구별 불가능하게 병합하는 구조적 모호성
- **digit-level-verbatim-retrieval**: 출판 수치의 자릿수 일치로 감사하는 최대 엄격 기억 검증 방법

## 🔗 관련 논문

- Revisiting Non-Verbatim Memorization in Large Language Model
- Knowledge Acquisition During Pre-training? Large Language Models Learn

## 🏷️ 엔티티

- [[entities/fact-memorization.md|fact-memorization]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/entity-surface-form.md|entity-surface-form]]
- [[entities/redirectqa.md|redirectqa]]
- [[entities/data-contamination-resistance.md|data-contamination-resistance]]
- [[entities/training-phase-knowledge-contamination.md|training-phase-knowledge-contamination]]

## 📐 개념

- [[concepts/digit-level-verbatim-retrieval.md|digit-level-verbatim-retrieval]]
- [[concepts/prediction-retrieval-ambiguity.md|prediction-retrieval-ambiguity]]
- [[concepts/benchmark-contamination-audit.md|benchmark-contamination-audit]]
- [[concepts/evaluator-assumption.md|evaluator-assumption]]
- [[concepts/ceiling-performance-problem.md|ceiling-performance-problem]]
- [[concepts/score-narrative-conflation.md|score-narrative-conflation]]

---
_LLM 분석으로 생성됨_
