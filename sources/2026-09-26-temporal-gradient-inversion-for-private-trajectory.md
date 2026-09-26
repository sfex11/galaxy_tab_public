# Temporal Gradient Inversion for Private Trajectory Reconstruction in Embodied Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-26
**링크**: http://arxiv.org/abs/2609.30258v1

## 💡 핵심 인사이트

그래디언트라는 간접 전송물이 프라이버시 경계가 아니라 유출 채널이며, 개별 스텝의 유출량이 아닌 시간적 상관 구조가 실제 복원 가능성을 결정한다.

## 📖 분석

# Temporal Gradient Inversion: 전송 계층 프라이버시 경계의 붕괴

## 정의

체화 RL의 표준 프라이버시 아키텍처는 '원시 센서 데이터는 디바이스에 유지하고 정책 그래디언트만 서버로 전송한다'는 전제 위에 성립한다. TRACE(Temporal Reconstruction Attack on Consecutive Encodings)는 이 전제를 반증한다 — 시점별 정책 그래디언트에서 사적 관찰-행동 궤적 전체를 자기회귀적으로 재구성하는 amortized temporal gradient inversion 공격이다.

## 핵심 발견

단일 프레임 공격으로는 위험을 과소평가한다. 연속 인코딩 간의 시간적 구조가 유출을 증폭시켜, 프레임별 복원의 단순 합을 넘는 궤적 수준 재구성이 가능해진다. 공격 자체가 자기회귀 디코딩이라는 점에서 모델 생성과 공격 재구성이 동일한 위상을 공유하는 역설도 주목할 만하다.

## 기존 Wiki와의 관계

- [[latent-communication-channel]], [[kv-cache-information-leakage]]: 그래디언트는 KV 캐시에 이어 또 하나의 비텍스트 유출 채널이다. 중간 표현이 관측 채널이 되는 동형 패턴이 제3 사례로 확장된다.
- [[differential-privacy]], [[federated-learning]]: Component-Aware DP가 방어 측 예산 배분이었다면 본 논문은 그 방어가 막아야 할 공격의 실재를 체화 RL에서 실증한다.
- [[hidden-state-risk-space]]: 위험이 출력 표층이 아닌 전송물에 거주한다는 위치 논리의 확장.
- [[efficiency-attack-surface-identity]]: 서버 조율을 위한 채널이 곧 공격 표면이 되는 이중성의 프라이버시 버전.

## 🔗 관련 논문

- Component-Aware Differential Privacy for Federated Multilingual Speech
- The Implications of Linguistic Illegibility for LLM Security
- Differential Privacy in Generative AI Agents: Analysis and Optimization
- LCGuard: Latent Communication Guard for Safe KV Sharing in M
- FL-PBM: Pre-Training Backdoor Mitigation for Federated Learning

## 🏷️ 엔티티

- [[entities/temporal-gradient-inversion.md|temporal-gradient-inversion]]
- [[entities/differential-privacy.md|differential-privacy]]
- [[entities/federated-learning.md|federated-learning]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/sensor-as-attack-surface.md|sensor-as-attack-surface]]

## 📐 개념

- [[concepts/temporal-structure-amplified-leakage.md|temporal-structure-amplified-leakage]]
- [[concepts/latent-communication-channel.md|latent-communication-channel]]
- [[concepts/kv-cache-information-leakage.md|kv-cache-information-leakage]]
- [[concepts/hidden-state-risk-space.md|hidden-state-risk-space]]
- [[concepts/linguistic-illegibility.md|linguistic-illegibility]]
- [[concepts/efficiency-attack-surface-identity.md|efficiency-attack-surface-identity]]

---
_LLM 분석으로 생성됨_
