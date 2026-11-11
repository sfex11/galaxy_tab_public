# REAL Loss: Optimizing Real Expected Acceptance Length for Speculative Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14399v1

## 💡 핵심 인사이트

추측 디코딩의 드래프트 훈련 목적은 분포 일치형 서로게이트가 아니라 배포 지표인 기대 수용 길이(EAL) 자체여야 하며, 이는 서빙 지표가 훈련 목적 함수를 정의하는 역방향 훈련-서빙 결합의 사례다.

## 📖 분석

REAL Loss는 추측 디코딩의 가속 이득을 지배하는 기대 수용 길이(Expected Acceptance Length, EAL)를 드래프트 모델 훈련의 직접 목적 함수로 삼는 손실을 제안한다. 교차 엔트로피·KL·TV 같은 표준 목적은 분포 일치나 단일 스텝 중첩만 보는 프록시였고, 최근의 블록 수준 목적도 여전히 EAL의 서로게이트에 머문다는 진단 위에서 EAL 자체의 최적화로 간극을 닫는다.

[[concepts/speculative-decoding.md|speculative-decoding]] 논의에 훈련 축의 새 층위를 추가한다 — 기존 위키가 런타임 γ 적응([[concepts/speculation-length-adaptation.md|speculation-length-adaptation]], [[concepts/compression-aware-gamma-selection.md|compression-aware-gamma-selection]])과 구조적 제약([[concepts/position-aware-drafting.md|position-aware-drafting]])으로 수용률을 개선했다면, 본 논문은 손실 함수 수준에서 수용률을 직접 겨냥하여 수용률 개선 수단이 런타임·구조·훈련의 3축으로 분화함을 확정한다.

[[concepts/training-serving-primitive-coupling.md|training-serving-primitive-coupling]]의 결합 논의에 역방향 사례를 제공한다 — 서빙 시점 지표(EAL)가 훈련 목적 함수를 직접 정의하여 결합이 '서빙이 훈련을 구속'에서 '서빙 지표가 훈련을 지시'로 진화한다. [[concepts/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]의 무손실 원칙(검증·기각 샘플링 불변)은 유지되되 드래프트의 위상이 '타겟의 축소 복제'에서 '수용 최적화 제안자'로 이동한다. 평가 축의 프록시 치환 문제([[concepts/evaluation-target-substitution.md|evaluation-target-substitution]])의 훈련 축 대응물을 진단·교정한 사례이기도 하다.

## 🔗 관련 논문

- Position-Aware Drafting for Inference Acceleration in LLM-Based Genera
- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Selection
- Watermarkable Multi-Draft Speculative Sampling via Poisson Processes

## 🏷️ 엔티티

- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/position-aware-drafting.md|position-aware-drafting]]
- [[entities/draft-model-domain-adaptation.md|draft-model-domain-adaptation]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/real-loss.md|real-loss]]

## 📐 개념

- [[concepts/expected-acceptance-length.md|expected-acceptance-length]]
- [[concepts/serving-metric-as-training-objective.md|serving-metric-as-training-objective]]
- [[concepts/verification-guarantee-boundary.md|verification-guarantee-boundary]]
- [[concepts/evaluation-target-substitution.md|evaluation-target-substitution]]
- [[concepts/training-serving-primitive-coupling.md|training-serving-primitive-coupling]]
- [[concepts/speculation-length-adaptation.md|speculation-length-adaptation]]
- [[concepts/compression-aware-gamma-selection.md|compression-aware-gamma-selection]]
- [[concepts/draft-policy-role-entanglement.md|draft-policy-role-entanglement]]

---
_LLM 분석으로 생성됨_
