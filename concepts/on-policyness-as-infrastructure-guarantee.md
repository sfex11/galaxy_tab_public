# 온폴리시성의 인프라 조건화

**생성일**: 2026-09-20

## 정의

온폴리시성은 알고리즘의 선언적 속성이 아니라, 훈련 엔진과 롤아웃 엔진 간 수치 일치(logits/샘플링 분포 일치도)라는 인프라 조건이 보장하는 속성이라는 재정의. TIM이 존재하면 문서상 on-policy 학습은 실제로는 암묵적 off-policy가 되며, 불안정의 원인이 알고리즘이 아닌 정밀도·커널·KV 관리 같은 인프라 구성에 위치한다.

## 관련 논문

- training-inference-mismatch
- score-centering
- adaptive-credit-granularity
- agentic-distillation
- algorithm-system-boundary-collapse

---
_자동 Wiki Query에서 추출됨_

### OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre (2026-09-21)

→ [[sources/2026-09-21-opted-on-policy-fine-tuning-for-end-to-end-driving.md|상세 보기]]

### Score Centering Stabilizes Off-policy Reinforcement Learning (2026-09-21)

→ [[sources/2026-09-21-score-centering-stabilizes-off-policy-reinforcemen.md|상세 보기]]
