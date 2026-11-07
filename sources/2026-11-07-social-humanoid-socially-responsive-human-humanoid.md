# Social Humanoid: Socially Responsive Human-Humanoid Interaction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08407v1

## 💡 핵심 인사이트

인간과의 물리적 사회 조율은 반응적 모방이 아니라 상호 예측이며, 이는 인간 모션과 로봇 모션을 공유 토큰 공간에서 함께 시퀀스 모델링함으로써 달성된다.

## 📖 분석

# Social Humanoid: Socially Responsive Human-Humanoid Interaction

휴머노이드가 단독 에이전트로 훈련되어 인간 파트너의 상호 예측·조정(anticipate and adjust)에 참여하지 못하는 문제를 진단하고, 29-DoF Unitree G1에서 인간 파트너 모션에 조건화된 사회적 반응 전신 모션을 생성·실행하는 계층형 시스템을 제시한다.

## 기존 Wiki와의 관계

**[[latent-aligned-planning]]의 대상 확장**: Continuous Actions from Discrete Minds가 이산 추론-연속 제어 간 공유 잠재 인터페이스를 제시했다면, 본 논문은 공유 토큰화 표현 위에서 인간 모션과 휴머노이드 모션을 함께 시퀀스 모델링하여 잠재 정렬의 대상을 에이전트 내부 계층에서 에이전트-인간 이종 궤적 쌍으로 확장한다.

**[[communication-free-coordination]]의 체화 실현**: 명시적 통신 없이 파트너 모션 관찰만으로 물리 조율이 성립한다. 다만 단순 모방([[copying-collective-behavior]])과 달리 상대의 미래 동작 예측을 전제하므로 [[theory-of-mind]]의 운동 도메인 버전을 요구한다.

**[[thought-action-separation]]**: 고수준 사회적 시퀀스 모델링과 저수준 전신 제어의 계층 분리가 사회적 반응성과 운동 정밀도의 이중 요구 해법으로 작동함을 실증한다.

**[[representation-action-gap]]**: 인간 모션 관찰을 29-DoF 휴머노이드 신체로 번역하는 문제는 관찰자-실행자 신체 이질성에서 발생하는 표현-행동 간극의 새 발현면이다.

## 새 개념 제안

- **anticipatory-social-coordination**: 상대 미래 동작 예측에 기반한 사전 조정의 쌍방향 동역학
- **shared-motion-token-space**: 인간-로봇 모션을 단일 토큰 공간에서 모델링하는 상호작용 표현 설계

## 🔗 관련 논문

- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- Copying explains the collective behavior of AI agents in the
- Where Should I Join? Robot Group Joining via Language-Guided
- Learning to Communicate: Toward End-to-End Optimization of M

## 🏷️ 엔티티

- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/latent-aligned-planning.md|latent-aligned-planning]]
- [[entities/action-tokenization.md|action-tokenization]]
- [[entities/communication-free-coordination.md|communication-free-coordination]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/agent-coordination.md|agent-coordination]]
- [[entities/representation-action-gap.md|representation-action-gap]]
- [[entities/low-frequency-planning-high-frequency-execution.md|low-frequency-planning-high-frequency-execution]]
- [[entities/anticipatory-social-coordination.md|anticipatory-social-coordination]]
- [[entities/shared-motion-token-space.md|shared-motion-token-space]]

## 📐 개념

- [[concepts/anticipatory-social-coordination.md|anticipatory-social-coordination]]
- [[concepts/shared-motion-token-space.md|shared-motion-token-space]]
- [[concepts/social-responsiveness.md|social-responsiveness]]
- [[concepts/partner-conditioned-motion-generation.md|partner-conditioned-motion-generation]]

---
_LLM 분석으로 생성됨_
