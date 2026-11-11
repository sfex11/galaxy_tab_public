# Pterodactyl: Pushing the Limits of Efficient Automated Translation Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14480v1

## 💡 핵심 인사이트

LLM judge의 신뢰성·비용 한계는 판정을 저차원 이진 트리아지로 축소함으로써 실무적으로 관리 가능해지며, 이로써 평가가 대규모 번역 데이터 큐레이션의 주도자로 전환된다.

## 📖 분석

# Pterodactyl: 효율 극한의 자동 번역 평가

2026년 WMT26 자동 품질 평가 공유 과제(1020 Group) 제출 시스템. 세그먼트 수준 품질 점수 예측과 오류 없는 세그먼트 탐지(2·3 서브태스크)를 위한 초저비용, 고커스터마이징 LLM-as-a-Judge 시스템으로, 번역 트리아지와 데이터 큐레이션용 이진 분류에 최적화되어 있다.

## Wiki와의 연결

**Judge의 측정기기화.** [[llm-as-judge]]를 절대 채점자가 아닌 저차원 이진 트리아지 필터로 재배치한다. [[judge-instrument-reliability]] 계열이 진단한 judge 비일관성([[transitivity-violation]] 포함) 문제에 대해, '얼마나 좋은가'에서 '오류가 있는가'로 판정 차원을 축소해 신뢰성-해상도 트레이드오프로 재정의하는 완화 경로를 제공한다.

**MT 평가의 의미 판단 전환.** [[meaning-insensitive-metric]] 비판(WER류 표면 지표의 의미 무감각성)에 대한 [[machine-translation]] 도메인 응답이다. 참조 번역 없이 세그먼트 수준 품질을 예측하는 번역 품질 추정(QE)의 LLM 실현으로, MT 평가가 표면 일치에서 의미 보존 판정으로 이동 중임을 확정한다.

**비용을 1급 제약으로.** 초저비용 설계는 [[cost-aware-agent-evaluation]] 원리를 평가 도구 자체에 적용한 사례다. 저비용 judge 덕에 평가가 데이터 큐레이션 규모로 확장되며, 이는 평가 결과가 훈련 데이터 선택을 필터링하는 [[evaluation-training-causal-closure]]의 양성 실현 사례이기도 하다.

## 🔗 관련 논문

- Evaluation of Automatic Speech Recognition Using Generative Large Lang
- Clean Engineering, Unstable Measurement: A Preregistered Reliability F

## 🏷️ 엔티티

- [[entities/machine-translation.md|machine-translation]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[entities/ptero-dactyl.md|ptero-dactyl]]
- [[entities/translation-quality-estimation.md|translation-quality-estimation]]

## 📐 개념

- [[concepts/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/transitivity-violation.md|transitivity-violation]]
- [[concepts/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[concepts/error-free-segment-detection.md|error-free-segment-detection]]
- [[concepts/conditional-reliability-recalibration.md|conditional-reliability-recalibration]]
- [[concepts/evaluation-training-causal-closure.md|evaluation-training-causal-closure]]

---
_LLM 분석으로 생성됨_
