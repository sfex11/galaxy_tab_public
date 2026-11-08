# SCALE: Real-Time Latent Communication for Cyber-Physical Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08390v1

## 💡 핵심 인사이트

잠재 통신의 병목은 채널 용량이 아니라 인코딩 설계이며, CPS 도메인의 대역폭·데드라인 제약이 통신 최적화의 목표 함수를 재정의한다.

## 📖 분석

SCALE은 잠재 통신(latent communication)을 LLM 에이전트 도메인에서 사이버-물리(CPS) 에이전트로 확장한다. 기존 접근([[entities/latent-inter-agent-communication.md|latent inter agent communication]])이 원시 센서 데이터·텍스트 대신 모델 중간 표현을 교환해 효율성을 얻었으나, CPS 도메인의 대역폭 제약과 이기종 태스크 데드라인은 고려하지 않았다. SCALE은 센서 데이터의 시공간 연속성([[concepts/spatio-temporal-continuity-encoding.md|spatio temporal continuity encoding]])을 활용해 실시간 표현 교환을 실현한다.

Wiki 기존 논의와의 두 접점이 있다. 첫째, [[entities/distributed-consensus-estimation.md|distributed consensus estimation]] 계열(파티클 필터)이 관측 데이터를 교환하던 분산 추정과 달리, 표현 수준 통신은 통신 병목을 채널 용량 문제에서 인코딩 설계 문제로 이동시킨다. 둘째, [[concepts/communication-reasoning-joint-optimization.md|communication reasoning joint optimization]]의 목표 함수에 이기종 데드라인이라는 CPS 고유의 시간 제약 축이 추가된다.

물리 신호가 갖는 자연적 접지 덕에 CPS 잠재 통신은 [[concepts/latent-communication-homogeneity-dependency.md|latent communication homogeneity dependency]]가 지적한 LLM 도메인의 가중치 동질성 의존을 우회할 수 있는 제2 경로를 열어, 잠재 통신의 유효 조건 논의를 확장한다.

## 🔗 관련 논문

- A Distributed Consensus Particle Filter for Target Tracking using Auto
- Learning to Communicate: Toward End-to-End Optimization of Multi-Agent

## 🏷️ 엔티티

- [[entities/cyber-physical-agent.md|cyber-physical-agent]]
- [[entities/scale.md|scale]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/distributed-consensus-estimation.md|distributed-consensus-estimation]]
- [[entities/communication-reasoning-joint-optimization.md|communication-reasoning-joint-optimization]]
- [[entities/spatio-temporal-continuity-encoding.md|spatio-temporal-continuity-encoding]]
- [[entities/deadline-aware-communication.md|deadline-aware-communication]]
- [[entities/bandwidth-constrained-latent-exchange.md|bandwidth-constrained-latent-exchange]]
- [[entities/latent-communication-homogeneity-dependency.md|latent-communication-homogeneity-dependency]]

## 📐 개념

- [[concepts/real-time-latent-communication.md|real-time-latent-communication]]
- [[concepts/latent-communication-channel.md|latent-communication-channel]]
- [[concepts/lossy-serialization-channel.md|lossy-serialization-channel]]

---
_LLM 분석으로 생성됨_
