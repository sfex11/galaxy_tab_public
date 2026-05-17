# Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy with Template Constrained Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-03
**링크**: http://arxiv.org/abs/2604.28028v1

## 💡 핵심 인사이트

반복 패턴을 학습 데이터가 아닌 디코딩 제약으로 재활용함으로써, 분포 변경 없이 출력 공간만 구조적으로 축소하여 신뢰성을 확보하는 추론 시점 제약 디코딩 패러다임을 제시한다.

## 📖 분석

# Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accuracy with Template Constrained Decoding

## 핵심 기여

TeCoD(Template Constrained Decoding)는 Text-to-SQL의 실제 배포 한계—스키마 복잡도에 따른 정확도 불일치와 무효 SQL 생성—를 해결하기 위해, 레이블링된 워크로드에서 반복되는 쿼리 패턴을 템플릿으로 변환하고 이를 디코딩 제약으로 활용한다. 드래프트 모델이 생성한 후보를 검증하는 speculative-decoding과 달리, TeCoD는 도메인 템플릿 자체를 제약원으로 삼아 출력 공간을 사전에 축소한다.

## 기존 Wiki와의 관계

**speculative-decoding과의 대비**: 기존 Wiki에서 speculative-decoding이 '드래프트 모델 기반 탐색 공간 축소'로 기술되었다면, TeCoD는 '도메인 템플릿 기반 제약 디코딩'이라는 대안적 경로를 제공한다. 제약원이 모델 내부(드래프트 모델의 분포)가 아닌 외부 도메인 지식(과거 성공 쿼리의 구조적 패턴)에 있을 때의 효과를 실증한다.

**marginal-distribution-ceiling과의 관계**: TeCoD는 타겟 분포 P(y|x)를 변경하지 않고 출력 공간만 제약하므로, 주변 분포 성능 상한선 원리를 준수하는 실제 구현 사례로 기능한다. 분포 외부로의 탐색 없이 분포 내부에서 최적점을 찾는 distribution-internal-optimization의 구체적 메커니즘이다.

**output-space-pruning의 실증**: 기존에 빈약했던 output-space-pruning 엔티티에 구체적 구현을 제공한다—템플릿 매칭을 통해 문법적으로 유효한 SQL 부분공간만을 남기고, 이 잔여 공간 내에서 LLM이 의미론적 완성을 수행하는 2단계 구조를 명확히 한다.

## 연결점

- [[entities/clawgym|ClawGym]]의 persistent-workspace-training이 에이전트 환경의 반복 패턴을 학습 데이터로 활용한다면, TeCoD는 SQL 워크로드의 반복 패턴을 디코딩 제약으로 활용한다—동일한 '반복성의 공학적 활용'이 서로 다른 계층(학습 vs 추론)에서 구현된 사례다.
- [[entities/crab|Crab]]의 재시도-컨텍스트 누적 문제를 TeCoD가 간접적으로 완화할 수 있다: 템플릿 제약이 첫 시도에서의 성공률을 높이므로 재시도 자체의 빈도를 감소시킨다.

## 🔗 관련 논문

- 2026-05-01-select-to-think-unlocking-slm-potential-with-local.md
- 2026-05-02-position-aware-drafting-for-inference-acceleration.md
- 2026-05-02-crab-a-semantics-aware-checkpointrestore-runtime-f.md
- 2026-05-01-clawgym-a-scalable-framework-for-building-effectiv.md

## 🏷️ 엔티티

- [[entities/text-to-sql.md|text-to-sql]]
- [[entities/template-constrained-decoding.md|template-constrained-decoding]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/output-space-pruning.md|output-space-pruning]]
- [[entities/query-pattern-recurrence.md|query-pattern-recurrence]]
- [[entities/distribution-internal-optimization.md|distribution-internal-optimization]]

## 📐 개념

- [[concepts/template-constrained-decoding.md|template-constrained-decoding]]
- [[concepts/query-pattern-recurrence.md|query-pattern-recurrence]]
- [[concepts/output-space-pruning.md|output-space-pruning]]
- [[concepts/distribution-internal-optimization.md|distribution-internal-optimization]]

---
_LLM 분석으로 생성됨_

---
**관련**: [[concepts/parallel-decoding.md|parallel decoding]]

---
**관련**: [[concepts/refusal-accuracy-dual-constraint.md|refusal accuracy dual constraint]]

---
**관련**: [[concepts/constrained-decoding.md|constrained decoding]]

---
**관련**: [[concepts/procedure-accuracy-decoupling.md|procedure accuracy decoupling]]
