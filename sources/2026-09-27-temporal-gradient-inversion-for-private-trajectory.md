# Temporal Gradient Inversion for Private Trajectory Reconstruction in Embodied Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-27
**링크**: http://arxiv.org/abs/2609.30258v1

## 💡 핵심 인사이트

프라이버시는 데이터의 위치가 아니라 전송되는 파생 표현의 시간적 구조로 결정된다 — 온디바이스 센서 격리 설계도, 연속 그래디언트에 남은 시간적 상관이 궤적 전체 복원을 가능하게 하면 무력하다.

## 📖 분석

# TRACE: 시간적 그래디언트 역전으로 프라이버시 바이 아키텍처를 무력화하다

분산 체화 RL에서 원시 센서를 디바이스에 보관하고 정책 그래디언트만 전송하는 설계는 표준적 프라이버시 방어다. TRACE(Temporal Reconstruction Attack on Consecutive Encodings)는 이 방어의 근본 한계를 보인다: 단계별 정책 그래디언트로부터 사유 관측-행동 궤적을 amortized 방식으로 자기회귀 복원한다.

핵심은 누출의 증폭 변수가 단일 프레임 정보량이 아니라 **시간적 구조**라는 점이다. 연속 인코딩 간 상관이 공격자에게 시간축 단서를 제공해, 개별 프레임으로는 불가능한 복원이 시퀀스 수준에서 가능해진다.

Wiki 지형에서의 위치:
- [[concepts/sensor-as-attack-surface.md|sensor as attack surface]]의 강력한 실증 — 물리적 센서 격리는 입력 계층 방어일 뿐, 파생 표현(그래디언트)이 새 공격 표면이 된다.
- [[concepts/hidden-state-risk-space.md|hidden state risk space]]의 확장 — 출력이 아닌 은닉 표현·그래디언트에 위험이 거주한다.
- [[concepts/temporal-structure-amplified-leakage.md|temporal structure amplified leakage]]의 원천 사례 — '무엇이 유출되는가'보다 '어떤 구조로 유출되는가'가 위험을 결정한다.
- [[concepts/latent-communication-channel.md|latent communication channel]]·[[concepts/kv-cache-information-leakage.md|kv cache information leakage]]와 결합하여, 잠재 계층의 독립적 보안이 훈련 전송 채널까지 요구됨을 확장한다.
- [[concepts/federated-learning.md|federated learning]]·[[concepts/differential-privacy.md|differential privacy]]에 대한 도전 — 연합 학습의 원시 데이터 국지 보관 전제가 무너지며, DP 노이즈가 시간적 상관 증폭을 충분히 파괴하는가가 새 설계 질문이 된다.

[[concepts/linguistic-illegibility.md|linguistic illegibility]]의 거울상이기도 하다: 텍스트-내부 단절은 방어 자원이 아니라, 내부를 직접 판독하는 공격자 앞에서 공격 비대칭으로 작동한다.

## 🔗 관련 논문

- Temporal Gradient Inversion for Private Trajectory Reconstruction in Embodied Reinforcement Learning
- The Implications of Linguistic Illegibility for LLM Security
- LCGuard: Latent Communication Guard for Safe KV Sharing in Multi-Agent Systems

## 🏷️ 엔티티

- [[entities/temporal-gradient-inversion.md|temporal-gradient-inversion]]
- [[entities/temporal-structure-amplified-leakage.md|temporal-structure-amplified-leakage]]
- [[entities/sensor-as-attack-surface.md|sensor-as-attack-surface]]
- [[entities/hidden-state-risk-space.md|hidden-state-risk-space]]
- [[entities/linguistic-illegibility.md|linguistic-illegibility]]
- [[entities/latent-communication-channel.md|latent-communication-channel]]
- [[entities/kv-cache-information-leakage.md|kv-cache-information-leakage]]
- [[entities/federated-learning.md|federated-learning]]

## 📐 개념

- [[concepts/differential-privacy.md|differential-privacy]]
- [[concepts/inference-privacy.md|inference-privacy]]
- [[concepts/temporal-structure-amplified-leakage.md|temporal-structure-amplified-leakage]]

---
_LLM 분석으로 생성됨_
