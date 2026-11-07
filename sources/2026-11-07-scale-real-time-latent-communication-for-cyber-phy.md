# SCALE: Real-Time Latent Communication for Cyber-Physical Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08390v1

## 💡 핵심 인사이트

잠재 통신이 LLM 에이전트의 효율화 기법에서 사이버-물리 에이전트의 실시간 제약(대역폭·데드라인) 하 필수 메커니즘으로 확장되며, 물리 세계의 시공간 연속성이 통신 압축의 새로운 근거가 된다.

## 📖 분석

SCALE은 잠재 통신을 LLM 에이전트에서 사이버-물리 에이전트(로봇·IoT)로 확장한다. 기존 [[latent-communication-channel]]·[[latent-inter-agent-communication]] 논의가 동질적 LLM 간 중간 표현 공유에 머물렀다면, 본 논문은 대역폭 제약과 이기종 태스크 데드라인이라는 실시간 제약 하에서 물리 에이전트가 중간 모델 표현을 직접 교환하는 방법을 제시한다.

세 축의 기여가 있다. (1) 통신 설계 변수에 실시간 제약을 명시 편입하여 [[communication-reasoning-joint-optimization]]에 실시간 시스템 축을 추가한다 — '무엇을 보낼지'가 대역폭 예산 하 인코딩 정책 문제로 구체화되며 [[communication-access-planning-gap]]의 물리 도메인 실증 무대를 넓힌다. (2) 물리 세계의 시공간 연속성을 압축의 근거로 삼아, [[distributed-consensus-estimation]] 계열이 원시 센서 데이터를 교환하던 분산 추정 패러다임을 표현 수준 통신으로 전환한다. (3) [[latent-communication-homogeneity-dependency]] 관점에서 센서 이종성이 강한 CPS 도메인은 동질성 전제의 최대 압력 지점으로, 본 논문의 성립 조건은 [[latent-island-fragmentation]]의 '잠재 섬 간 자연어 프로토콜 교량 필요성' 진단에 대한 물리 도메인 반증 후보가 된다.

Latent-Lens의 [[modality-crossing-latent-communication]]과 함께, 잠재 통신이 텍스트·LLM 한계를 넘어 모달리티·도메인을 가로지르는 범용 인프라로 이동 중임을 확정한다. [[agent-coordination]]의 통신 비용 구조도 표현 압축으로 관리 가능해지는 방향이 열린다.

## 🔗 관련 논문

- Learning to Communicate: Toward End-to-End Optimization of Multi-Agent Communication
- Recursive Multi-Agent Systems
- A Distributed Consensus Particle Filter for Target Tracking using AutoNOMOS
- Latent-Lens: Visual Perception in Small Language Models Through Latent Alignment
- Towards Communication-Efficient Social Intelligence in Language Agents
- The Natural Language Interaction Protocol and Standard for AI Agents

## 🏷️ 엔티티

- [[entities/scale.md|scale]]
- [[entities/cyber-physical-agent.md|cyber-physical-agent]]
- [[entities/latent-communication-channel.md|latent-communication-channel]]
- [[entities/latent-inter-agent-communication.md|latent-inter-agent-communication]]
- [[entities/agent-coordination.md|agent-coordination]]
- [[entities/communication-reasoning-joint-optimization.md|communication-reasoning-joint-optimization]]
- [[entities/communication-access-planning-gap.md|communication-access-planning-gap]]
- [[entities/latent-communication-homogeneity-dependency.md|latent-communication-homogeneity-dependency]]
- [[entities/distributed-consensus-estimation.md|distributed-consensus-estimation]]

## 📐 개념

- [[concepts/real-time-latent-communication.md|real-time-latent-communication]]
- [[concepts/bandwidth-constrained-latent-exchange.md|bandwidth-constrained-latent-exchange]]
- [[concepts/deadline-aware-communication.md|deadline-aware-communication]]
- [[concepts/spatio-temporal-continuity-encoding.md|spatio-temporal-continuity-encoding]]

---
_LLM 분석으로 생성됨_
