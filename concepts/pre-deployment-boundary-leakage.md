# 배포 이전부터의 훈련-추론 경계 누수

**생성일**: 2026-09-30

## 정의

배포 시점의 '고정 하네스'에 이미 훈련의 산물(예: 학습된 VQ-VAE 토크나이저 등 표현 계약)이 내장되어 있으므로, 훈련/추론 분리는 테스트 타임 학습 이전부터 구조적으로 누수되어 있었다는 관찰.

## 관련 논문

- action-tokenization
- agent-native-serving
- harness-learning
- training-inference-mismatch

---
_자동 Wiki Query에서 추출됨_
