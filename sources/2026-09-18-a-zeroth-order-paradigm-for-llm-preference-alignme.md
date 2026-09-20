# A Zeroth-Order Paradigm for LLM Preference Alignment

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19144v1

## 💡 핵심 인사이트

선호 정렬에서 우도 경사 대신 비교 오라클만으로 방향성 정보를 추출하면 우도 이동을 회피할 수 있으며, 이는 정렬 신호가 우도 모델링과 구조적으로 분리 가능한 독립 축임을 보여준다.

## 📖 분석

## A Zeroth-Order Paradigm for LLM Preference Alignment (2026-09-18)

DPO 계열 직접 선호 정렬의 계산·메모리 효율성을 유지하면서 우도 이동(likelihood displacement)을 회피하는 제로스-오더 정렬 방법론 ComPO(Comparison-based Preference Optimization)를 제안한다.

핵심은 정렬 신호의 패러다임 전환이다. 기존 방법은 선호 쌍을 우도 경사의 원료로 취급하여, 우도 마진이 작은 쌍에서 선호 응답의 우도마저 감소시키는 병리가 발생한다. ComPO는 선호 쌍을 비교 오라클(comparison oracle)의 출력으로 재해석해 우도 값이 아닌 쌍 간 방향성 정보만 추출한다.

이는 [[concepts/llm-alignment.md|llm alignment]]에 '비교 기반' 최적화 축을 추가하고, [[concepts/relative-verifiability.md|relative verifiability]]가 다룬 상대적 신호의 극한 형태 — 절대 값 없이 비교만으로 학습 — 를 정렬 도메인에서 실현한다. [[concepts/grpo.md|grpo]]가 그룹 비교로 advantage를 구성한다면, ComPO는 쌍 비교로 더 원자적 단위에서 동일 원리를 수행한다. [[concepts/positive-only-policy-optimization.md|positive only policy optimization]]과 함께 제한적 피드백 하 견고한 신호 추출이라는 공통 축을 형성한다.

우도 모델링과 정렬 신호의 구조적 분리 가능성이 이 논문이 후속 연구에 던지는 핵심 질문이다.

## 🔗 관련 논문

- Beyond Negative Rollouts: Positive-Only Policy Optimization with Implicit Negative Gradients

## 🏷️ 엔티티

- [[entities/llm-alignment.md|llm-alignment]]
- [[entities/relative-verifiability.md|relative-verifiability]]
- [[entities/grpo.md|grpo]]
- [[entities/positive-only-policy-optimization.md|positive-only-policy-optimization]]

## 📐 개념

- [[concepts/comparison-oracle.md|comparison-oracle]]
- [[concepts/likelihood-displacement.md|likelihood-displacement]]
- [[concepts/zeroth-order-preference-alignment.md|zeroth-order-preference-alignment]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-17-coupled-calibration-and-learning-mitigating-teache]]: 증류의 교사 편향과 정렬의 우도 이동이라는 훈련 신호의 체계적 왜곡을, 캘리브레이션 결합과 비교 기반 제로스-오더 방법으로 각각 교정한다.
