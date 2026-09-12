# Domain-Specific Hallucination Detection in Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11878v1

## 💡 핵심 인사이트

환각 감지에서 단일 신호는 불충분하며, 분류·불확실성·보정이라는 이질적 신호들의 융합이 각 신호가 놓치는 실패 모드를 상호 보완한다.

## 📖 분석

본 논문은 LLM 환각의 사후 감지를 위한 다중 신호 파이프라인을 제시한다. 미세조정된 DeBERTa-v3 분류기, MC Dropout 불확실성 정량화, 온도 스케일링 보정을 결합하여 응답 수준(response-level) 환각을 감지하며, HaluEval에서 F1=0.915·AUROC=0.977을 달성한다(QA 0.97, 요약 0.96).

기존 Wiki 축적과의 관계: Wiki는 환각의 생성 메커니즘(SFT 기반 환각, 학습 시점 지식 오염, 사실 접근-저장 분리)을 집중 다루어 왔으나, 본 논문은 감지 축을 제공하여 메커니즘-감지의 양축을 완성한다. 다중 신호 융합 구조는 단일 표면 신호의 불충분성 원칙의 구현 사례다 — 분류기 점수, 예측 분산(MC Dropout), 보정 신뢰도가 각각 이질적 실패 모드를 포착한다.

MC Dropout의 다중 순전파는 동의 기반 신뢰성의 파라미터 공간 버전으로, 출력 샘플링 대신 dropout 마스크 변이로 합의를 관찰한다. 응답 수준 입도는 토큰 수준 감지와 인용 감지(주장 수준, ReCite) 사이의 중간 축을 형성하며 감지 입도의 계층화 논의에 새 축을 추가한다. 도메인별 F1 편차는 태스크 유형이 환각 감지 용이성을 조건화함을 시사한다.

## 🔗 관련 논문

- MoRFI: Monotonic Sparse Autoencoder Feature Identification
- ReCite: Agentic Reasoning for Faithful Citation

## 🏷️ 엔티티

- [[entities/uncertainty-quantification.md|uncertainty-quantification]]
- [[entities/sft-hallucination-mechanism.md|sft-hallucination-mechanism]]
- [[entities/closed-book-qa-hallucination.md|closed-book-qa-hallucination]]
- [[entities/multi-signal-hallucination-detection.md|multi-signal-hallucination-detection]]
- [[entities/temperature-scaled-calibration.md|temperature-scaled-calibration]]

## 📐 개념

- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/agreement-based-reliability.md|agreement-based-reliability]]
- [[concepts/relative-verifiability.md|relative-verifiability]]
- [[concepts/measurement-repeatability.md|measurement-repeatability]]

---
_LLM 분석으로 생성됨_
