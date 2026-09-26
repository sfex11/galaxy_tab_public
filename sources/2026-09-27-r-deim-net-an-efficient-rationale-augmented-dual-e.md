# R-DEIM Net: An Efficient Rationale-Augmented Dual-Expert Interaction Model for Paraphrase Detection

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30100v1

## 💡 핵심 인사이트

76M 규모의 이중 전문가 구조는 경쟁적 정확도와 근거 생성의 양립을 입증하지만, 판정과 설명의 구조적 분리는 생성된 근거를 판정 계산과 단절된 '번역된 보고서'로 만들어 투명성 주장에 충실도 검증이라는 조건을 부과한다.

## 📖 분석

R-DEIM Net은 76M 파라미터 이중 전문가 아키텍처로 패러프레이즈 검출에서 경쟁적 정확도와 인간 가독형 근거 생성을 동시 추구하며, 기존 Wiki에 2026-09-26 등록된 엔트리의 본문 분석을 완성한다. 두 축에서 위키 논의와 접촉한다. 첫째, 소형 모델 능력 논의([[slm-reasoning-gap]])에 '과제 적합 규모 + 근거 생성 내장'이라는 경로를 추가한다 — Distill Globally가 추론 필요성 자체를 제거했다면, 본 논문은 근거 생성을 소형 모델의 일급 기능으로 격상시켜 [[marginal-distribution-ceiling]]의 실용적 상한을 탐색한다. 둘째, 투명성 주장의 비판적 감사 지점을 제공한다. 이중 전문가 구조는 판정과 설명을 별도 전문가가 담당하므로, 생성 근거는 구조적으로 판정 계산과 분리된 '번역된 보고서'([[cot-as-translated-report]])가 되며, [[legibility-interpretability-gap]] 원리상 가독성이 충실도를 보증하지 않는다. 76M 규모 선택은 LLM 중심 패러다임에 대한 실용적 도전으로서 비용-투명성 프론티어를 재정의한다.

## 🔗 관련 논문

- Distill Globally, Adapt Locally: Reasoning Distillation and 
- Legibility is Not Interpretability: Comparing Judged and Actual Import
- When LLM Decompilers Recompile More and Preserve Less

## 🏷️ 엔티티

- [[entities/efficient-paraphrase-detection.md|efficient-paraphrase-detection]]
- [[entities/rationale-augmented-detection.md|rationale-augmented-detection]]
- [[entities/dual-expert-judgment-explanation-split.md|dual-expert-judgment-explanation-split]]
- [[entities/moderate-scale-transparent-model.md|moderate-scale-transparent-model]]

## 📐 개념

- [[concepts/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]

---
_LLM 분석으로 생성됨_
