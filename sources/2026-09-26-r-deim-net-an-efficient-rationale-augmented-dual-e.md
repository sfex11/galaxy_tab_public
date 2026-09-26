# R-DEIM Net: An Efficient Rationale-Augmented Dual-Expert Interaction Model for Paraphrase Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30100v1

## 💡 핵심 인사이트

근거 생성을 판단 전문가와 분리된 별도 전문가에 위임하는 구조가, 소형 모델에서 정확도-투명성 트레이드오프의 구조적 완화 경로가 될 수 있음을 시사한다.

## 📖 분석

R-DEIM Net은 패러프레이즈 검출에서 LLM의 높은 정확도와 Siamese-BERT 계열의 효율성 사이 트레이드오프를 76M 파라미터의 듀얼 익스퍼트 구조로 타결을 시도한다. 핵심 설계는 판단 전문가와 근거(rationale) 생성 전문가를 분리하여, 중간 규모 모델에서도 인간 판독 가능한 설명을 산출하게 하는 것이다.

이 논문은 기존 Wiki 논의에 두 축을 추가한다. 첫째, [[legibility-interpretability-gap]] 계열의 진단에 대응하는 구조적 해법 후보를 제시한다 — Legibility is Not Interpretability가 '가독적 근거가 실제 이유를 담보하지 않는다'고 진단했다면, 본 논문은 근거 생성을 별도 전문가에 위임함으로써 판단 경로와 설명 경로의 분리를 명시화한다. 다만 생성된 근거가 실제 판단 과정을 반영하는지는 여전히 검증 과제로 남아, [[cot-as-translated-report]]의 인식론적 규정이 그대로 적용된다.

둘째, [[slm-reasoning-gap]] 논의에 패러프레이즈 도메인의 실증 사례를 제공한다. 소형 모델의 추론 격차를 능력 향상이 아닌 '판단-설명 분리'라는 아키텍처 선택으로 완화하는 경로는, Select to Think의 국소 충분성 기반 선택과 병렬되는 구조적 완화 전략이다. 듀얼 익스퍼트 구조는 [[thought-action-separation]]의 판단-설명 버전으로 해석 가능하며, 전문가 분리가 저비용 도메인에서도 효과적인지의 경계를 탐색한다.

## 🏷️ 엔티티

- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/model-compression.md|model-compression]]
- [[entities/rationale-augmented-detection.md|rationale-augmented-detection]]

## 📐 개념

- [[concepts/rationale-augmented-detection.md|rationale-augmented-detection]]
- [[concepts/dual-expert-judgment-explanation-split.md|dual-expert-judgment-explanation-split]]
- [[concepts/efficient-paraphrase-detection.md|efficient-paraphrase-detection]]
- [[concepts/moderate-scale-transparent-model.md|moderate-scale-transparent-model]]

---
_LLM 분석으로 생성됨_
