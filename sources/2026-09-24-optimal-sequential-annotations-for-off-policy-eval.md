# Optimal Sequential Annotations for Off-Policy Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26707v1

## 💡 핵심 인사이트

오프폴리시 평가에서 저비용·편향 LLM 주석과 고비용·신뢰 전문가 주석의 최적 순차 결합은 '교정 근거의 구매 위치' 자체를 최적화 문제로 만들어, LLM judge를 폐기하지 않고 통계적으로 구제하는 교정 기반 신뢰성 경로를 연다.

## 📖 분석

오프라인 강화학습과 오프폴리시 평가(OPE)에서 상태·보상이 복잡한 텍스트·이미지로 기록되는 AI 응용을 대상으로, 저비용이지만 알 수 없는 편향을 가진 라벨러(LLM-as-a-judge, 저렴한 분류기)와 고비용·고신뢰 전문가 주석을 순차적으로 최적 결합하여 동적 치료 규칙을 평가하는 통계 프레임워크를 제시한다.

[[prediction-powered-inference]] 계열이 소량의 고정 라벨로 모델 예측을 교정하는 정적 구조였다면, 본 논문은 '어느 표본에 비싼 전문가 라벨을 구매할 것인가'를 순차 최적화 문제로 형식화한다. 이는 [[expected-value-of-information]]의 적용 영역을 도구 호출에서 주석 획득으로 확장하는 사례다 — 전문가 라벨의 기대 정보 가치가 비용을 넘을 때만 구매하는 정책이 된다.

[[llm-as-judge]]의 위상에 제3의 경로를 연다. judge를 신뢰할 수 없는 측정기로 폐기하거나([[black-box-instrument-drift]]), 다중 신호 합의로 우회하거나([[agreement-based-reliability]]) 하는 대신, 소량의 모델-독립 골드 스탠다드로 judge 편향을 통계적으로 보정하는 교정 기반 신뢰성 경로다. 전문가 주석은 [[verification-as-system-external-relation]]의 유료·희소 실현이며, 안전 분류 예시는 [[human-oversight]]를 '감독을 어느 표본에 배분할까'라는 예산 최적화 문제로 재정의한다.

## 🔗 관련 논문

- Prediction-Powered Smoothing and Validation for Disaggregated AI Evalu
- Clean Engineering, Unstable Measurement: A Preregistered Reliability F
- Why Global LLM Leaderboards Are Misleading: Small Portfolios

## 🏷️ 엔티티

- [[entities/off-policy-evaluation.md|off-policy-evaluation]]
- [[entities/sequential-annotation-optimization.md|sequential-annotation-optimization]]
- [[entities/prediction-powered-inference.md|prediction-powered-inference]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/human-oversight.md|human-oversight]]
- [[entities/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[entities/agreement-based-reliability.md|agreement-based-reliability]]
- [[entities/black-box-instrument-drift.md|black-box-instrument-drift]]

## 📐 개념

- [[concepts/llm-as-annotator.md|llm-as-annotator]]
- [[concepts/annotation-budget-allocation.md|annotation-budget-allocation]]
- [[concepts/bias-correction-with-gold-standard.md|bias-correction-with-gold-standard]]
- [[concepts/sequential-information-purchase.md|sequential-information-purchase]]
- [[concepts/dynamic-treatment-rule-evaluation.md|dynamic-treatment-rule-evaluation]]

---
_LLM 분석으로 생성됨_
