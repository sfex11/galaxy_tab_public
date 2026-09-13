# Domain-Specific Hallucination Detection in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-13
**링크**: http://arxiv.org/abs/2609.11878v1

## 💡 핵심 인사이트

환각 감지는 단일 신호의 정밀도 문제가 아니라 의미 분류·인식론적 불확실성·보정이라는 직교하는 측정 신호의 결합 문제이며, 이 3축 융합이 HaluEval에서 F1=0.915/AUROC=0.977로 그 우월성을 실증한다.

## 📖 분석

## Domain-Specific Hallucination Detection in Large Language Models (2026-09-13)

미세조정 DeBERTa-v3 분류기, MC Dropout 불확실성 정량화, 온도 스케일링 보정을 결합한 응답 수준(response-level) 환각 감지 파이프라인을 제시한다. HaluEval 벤치마크에서 일반 도메인 F1=0.915, AUROC=0.977을 달성하며, QA(F1 0.97)와 요약(F1 0.96) 등 태스크별 성능 편차가 존재함을 보여준다.

핵심 기여는 '환각 감지'를 단일 신호의 정밀도 문제가 아닌 **측정 문제**로 재정의한 점이다. 의미 분류(무엇이 거짓인가), 인식론적 불확실성(모델이 얼마나 확신하는가), 보정(확신이 실제 정확도와 일치하는가)의 세 축이 직교하는 정보를 제공하며, 이들의 결합이 단일 최강 신호보다 우월함을 실증한다.

→ [[entities/multi-signal-hallucination-detection.md|multi signal hallucination detection]]: 이 엔티티의 원천 구현 사례. 분류·불확실성·보정의 3신호 구성을 조작적 정의로 확립한다.

→ [[entities/temperature-scaled-calibration.md|temperature scaled calibration]]: 온도 스케일링이 보정 계층의 구체적 구현으로 채택되어 모델 과신을 교정함을 보여준다.

→ [[concepts/closed-book-qa-hallucination.md|closed book qa hallucination]]: QA 도메인 F1 0.97은 폐쇄형 질의응답 환각이 사후 감지로 관찰 가능함을 정량화한다.

→ [[concepts/sft-hallucination-mechanism.md|sft hallucination mechanism]]: 환각 생성 메커니즘 연구가 감지 파이프라인 설계의 경험적 근거가 됨을 시사한다.

→ [[concepts/measurement-repeatability.md|measurement repeatability]]: 감지기를 측정 기기로 취급할 때 다중 신호 결합이 측정 안정성을 높이는 기제로 작동함을 부각한다.

→ [[concepts/uncertainty-quantification.md|uncertainty quantification]]: MC Dropout이 출력 수준 불확실성의 경량 구현 경로임을 실증한다.

→ [[concepts/black-box-instrument-drift.md|black box instrument drift]]: 미세조정 분류기 자체가 드리프트 가능성을 지닌 블랙박스 측정 기기임을 시사한다.

→ [[concepts/agreement-based-reliability.md|agreement based reliability]]: 다중 독립 신호 간 합의가 단일 판단보다 신뢰로 이어지는 원리를 환각 도메인에서 확인한다.

## 🔗 관련 논문

- Domain-Specific Hallucination Detection in Large Language Models
- Forgetting Only What Matters: Layer-Selective Unlearning toward Robust
- Legibility is Not Interpretability: Comparing Judged and Actual Import

## 🏷️ 엔티티

- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/temperature-scaled-calibration.md|temperature-scaled-calibration]]
- [[entities/closed-book-qa-hallucination.md|closed-book-qa-hallucination]]
- [[entities/sft-hallucination-mechanism.md|sft-hallucination-mechanism]]
- [[entities/uncertainty-quantification.md|uncertainty-quantification]]
- [[entities/measurement-repeatability.md|measurement-repeatability]]
- [[entities/black-box-instrument-drift.md|black-box-instrument-drift]]
- [[entities/agreement-based-reliability.md|agreement-based-reliability]]

## 📐 개념

- [[concepts/mc-dropout-uncertainty.md|mc-dropout-uncertainty]]
- [[concepts/response-level-hallucination-detection.md|response-level-hallucination-detection]]
- [[concepts/halu-eval-benchmark-evaluation.md|halu-eval-benchmark-evaluation]]
- [[concepts/orthogonal-signal-fusion.md|orthogonal-signal-fusion]]
- [[concepts/detector-as-instrument.md|detector-as-instrument]]

---
_LLM 분석으로 생성됨_
