# Social Humanoid: Socially Responsive Human-Humanoid Interaction

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08407v1

## 💡 핵심 인사이트

사회적 물리 조율은 명시적 통신이 아니라 이종 신체를 통일한 공유 토큰 공간 위의 상대 모션 예측으로 성립하며, 파트너의 실시간 모션이 생성의 조건 변수가 되는 순간 휴머노이드가 사회적 상호작용의 일등 참여자가 된다.

## 📖 분석

# Social Humanoid: Socially Responsive Human-Humanoid Interaction (2026-11-08)

휴머노이드를 단독 에이전트로 훈련하는 관행이, 서로를 예측하고 조정하는 인간 파트너의 자연적 사회성에 물리적으로 응답하지 못하게 하는 구조적 한계를 진단한다. 29-DoF Unitree G1에서 인간 파트너의 모션에 조건화된 사회적 반응형 전신 동작을 생성·실행하는 계층형 시스템을 제시한다.

## 아키텍처와 Wiki 연결

- **고수준 정책**: 인간·휴머노이드 모션을 공유 토큰 표현으로 유연하게 시퀀스 모델링 ([[concepts/shared-motion-token-space.md|shared motion token space]])
- **저수준**: 전신 물리 제어 — [[concepts/low-frequency-planning-high-frequency-execution.md|low frequency planning high frequency execution]]의 주파수 분리가 휴머노이드 도메인에서 구현된 사례

## Wiki 내 위치

1. [[concepts/anticipatory-social-coordination.md|anticipatory social coordination]]의 원천: 사회적 조율을 반응적 추종이 아닌 '상대 미래 동작의 예측적 생성'으로 정의한다.
2. [[concepts/communication-free-coordination.md|communication free coordination]] 확장: 명시적 통신 채널 없이 파트너 모션 관찰만으로 전신 조율이 성립하는 인간-휴머노이드 쌍을 무통신 조율 스펙트럼에 추가한다 (Formation Matrix의 에너지 기반 무통신 형성 제어와 병렬).
3. [[concepts/partner-conditioned-motion-generation.md|partner conditioned motion generation]]: 모션 생성의 조건 변수가 텍스트 목표에서 상대의 실시간 모션 스트림으로 이동함을 실증한다.

## 연결점

- **IMPACT**(2026-10-01): 사회적 상호의존 이동 모델링이 생성 시뮬레이션에서 물리 체화 도메인으로 확장됨
- **Where Should I Join?**(2026-09-25): 로봇의 사회적 공간 추론에 물리적 상호 조율 차원을 추가
- **Mind2Dialogue**(2026-09-16): human-aware 훈련의 체화 버전 — 인간 인식이 텍스트를 넘어 모션 스트림에서 학습 가능함을 보인다

**핵심 명제**: 이종 신체(인간-휴머노이드)를 단일 토큰 공간으로 통일하면 사회적 상호 예측이 학습 가능한 시퀀스 모델링 문제로 환원되고, 파트너의 모션이 생성의 조건 변수가 되는 순간 휴머노이드는 사회적 상호작용의 일등 참여자가 된다.

## 🔗 관련 논문

- IMPACT: Modeling Socially Interdependent Movement in a Generative Multi-Agent Simulation
- Where Should I Join? Robot Group Joining via Language-Guided Goal Prediction
- Mind2Dialogue: Training Human-Aware Language Models by Simulating Users
- Formation Matrix and Energy-based Control of Multi-Agent Systems
- Learning to Communicate: Toward End-to-End Optimization of Multi-Agent Communication
- Visually-grounded Humanoid Agents

## 🏷️ 엔티티

- [[entities/social-humanoid.md|social-humanoid]]
- [[entities/anticipatory-social-coordination.md|anticipatory-social-coordination]]
- [[entities/social-responsiveness.md|social-responsiveness]]
- [[entities/shared-motion-token-space.md|shared-motion-token-space]]
- [[entities/partner-conditioned-motion-generation.md|partner-conditioned-motion-generation]]
- [[entities/humanoid-agent.md|humanoid-agent]]

## 📐 개념

- [[concepts/anticipatory-social-coordination.md|anticipatory-social-coordination]]
- [[concepts/social-responsiveness.md|social-responsiveness]]
- [[concepts/shared-motion-token-space.md|shared-motion-token-space]]
- [[concepts/partner-conditioned-motion-generation.md|partner-conditioned-motion-generation]]
- [[concepts/low-frequency-planning-high-frequency-execution.md|low-frequency-planning-high-frequency-execution]]
- [[concepts/communication-free-coordination.md|communication-free-coordination]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/humanoid-agent.md|humanoid-agent]]

---
_LLM 분석으로 생성됨_
