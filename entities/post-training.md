# post-training

**카테고리**: 미분류
**생성일**: 2026-05-01

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-01-morfi-monotonic-sparse-autoencoder-feature-identif.md|MoRFI: Monotonic Sparse Autoencoder Feature Identification]]

### Exploration Hacking: Can LLMs Learn to Resist RL Training? (2026-05-02)

RL 기반 사후학습이 가진 자기참조적 취약성을 최초로 명시적으로 문제화한다. 사후학습 안전성이 보상 모델 품질로 환원 불가함을 보여주며, 탐색 과정 자체에 대한 검증이 필요함을 시사한다.

### Exploration Hacking: Can LLMs Learn to Resist RL Training? (2026-05-03)

RL 기반 사후학습이 가진 자기참조적 취약성을 최초로 명시적으로 문제화한다. 사후학습 안전성이 보상 모델 품질로 환원 불가함을 보여주며, 탐색 과정 자체에 대한 독립적 검증이 필요함을 시사한다.

### Optimizer-Model Consistency: Full Finetuning with the Same Optimizer a (2026-05-10)

사후학습의 안정성이 RL 기반 보상 설계뿐 아니라 SFT 단계의 옵티마이저-사전학습 일관성에 의해서도 결정됨을 보여주며, 탐색 해킹과 같은 고차원적 취약성뿐 아니라 가장 기초적인 훈련 설정에서도 사후학습의 자기참조적 불안정이 발생할 수 있음을 시사한다.

### Beyond Negative Rollouts: Positive-Only Policy Optimization with Impli (2026-05-10)

### Crafting Reversible SFT Behaviors in Large Language Models (2026-05-10)

SFT가 행동을 모델에 유도할 때 그 행동의 내부 분포에 구조적 제약을 부과하지 않는다는 근본적 한계를 최초로 형식화하며, 이것이 사후학습 행동의 인과적 비가역성을 낳는 원인임을 밝힌다.

### Cliff: Learning Process Rewards from the First Mistake (2026-09-04)

PRM 학습이나 온폴리시 증류 같은 별도 파이프라인 없이, 기존 결과 보상 신호에서 프로세스 수준 가이드를 추출하는 post-training의 경량화 설계를 제시한다. 기존 post-training 스펙트럼(RL, 증류, PRM)에 '보상 분해 기반' 제4의 경로를 추가한다.

### Post-Training Language Models for Gold-Medal Performance in Coding Com (2026-09-04)

문제 큐레이션(22,000개)→합성 검증 트레이스→SFT→RL로 이어지는 완결적 도메인 특화 파이프라인을 제시하여, post-training이 사전학습 능력의 정제가 아닌 경쟁급 능력의 창출 경로임을 IOI·ICPC 금메달 수준에서 실증한다.

### Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E (2026-09-06)

포스트트레이닝의 실제 요구가 데이터가 아닌 환경임을 규정한다 — 환경은 다중 검증 가능 태스크와 실행 피드백을 제공하는 반면 궤적은 고정 데모에 불과하다는 구조적 대비를 확립한다.

### SpecGuard: Inference-Time Backdoor Detection For Free (2026-09-12)

서드파티 파인튜닝이 백도어의 주요 유입 경로임을 전제로, 유입 차단이 아닌 출구 감시라는 상보적 대응을 제시한다. 포스트트레이닝 파이프라인의 신뢰 가정이 깨질 수 있음을 인정하면서도 런타임 계층에서 이를 보완하는 설계다.

→ [[sources/2026-09-12-specguard-inference-time-backdoor-detection-for-fr.md|상세 보기]]

### LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language  (2026-09-12)

포스트트레이닝 업데이트의 파라미터화(저랭크 부공간 선택)가 생성 행동(길이)의 인과 제어 변수임을 밝힘. 기존 포스트트레이닝 논의가 '무엇을 학습시킬까'(손실·데이터·방법)에 머물렀다면, 본 논문은 '어떤 표현 공간에서 학습시킬까'라는 제2의 설계 축을 제시하며, 선호 정렬이 유틸리티 개선 없이 장황함을 부풀린다는 진단과 함께 그 보정 경로를 제공한다.

→ [[sources/2026-09-12-locus-task-aware-low-rank-post-training-for-token-.md|상세 보기]]
