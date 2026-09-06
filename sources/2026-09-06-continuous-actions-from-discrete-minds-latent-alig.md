# Continuous Actions from Discrete Minds: Latent-Aligned Planning for End-to-End Autonomous Driving

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04070v1

## 💡 핵심 인사이트

VLM의 이산적 추론과 자율주행의 연속적·물리제약 동역학 사이의 간극은 언어 수준의 사고 확장이 아니라 잔차 VQ-VAE 행동 토큰화와 잠재 공간 정렬을 통해 표현 형식 수준에서 해결되어야 한다.

## 📖 분석

LaPla는 VLM의 이산적 추론(discrete minds)과 자율주행의 연속적·물리제약 동역학 사이의 표현 형식 간극을 해결하는 통합 Vision-Language-Action 프레임워크다. 잔차 VQ-VAE 기반 action tokenizer가 차량 kinematics를 이산 토큰으로 변환하면서 연속성의 정밀도를 보존하고, latent-aligned planning이 의미론적 이해 공간과 모션 실행 공간을 잠재 차원에서 정렬한다.

이 논문은 [[thinking-acting-gap]]을 '사고의 양' 문제에서 '표현 형식의 질' 문제로 재정의한다. 기존 연구가 행동 공간의 탐색·검증에 집중했다면, LaPla는 간극의 근원이 이산-연속 표현 경계 자체에 있음을 지적한다. 이는 [[senses-wide-shut]]이 진단한 [[representation-action-gap]]의 극단적 사례로, 언어 추론은 정확하나 연속적 제어 신호 생성에서 실패하는 구조를 잔차 양자화로 봉합한다.

[[vla-foundry]]·[[end-to-end-vla-training]] 계보에 자율주행이라는 연속적 제약 도메인을 추가하여 VLA의 스코프를 조작에서 차량 제어로 확장한다. [[vector-quantization]]의 적용 대상을 내부 표현 제어에서 행동 토큰화로 이동시키며, [[semantic-id-tokenization]]과 함께 '비텍스트 대상의 이산 토큰화'라는 공통 패턴을 형성한다. [[algorithm-system-translation-gap]] 관점에서 잠재 공간 정렬은 의미론(상단)과 실행(하단) 사이에 새로운 중간 표현 계층을 삽입하는 번역 해법이다.

## 🔗 관련 논문

- Toward Robust LiDAR Semantic Segmentation for Real-World Deployment: E
- VLA Foundry: A Unified Framework for Training Vision-Languag
- Agent Explorative Policy Optimization for Multimod
- Learning to Communicate: Toward End-to-End Optimization of M

## 🏷️ 엔티티

- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/thinking-acting-gap.md|thinking-acting-gap]]
- [[entities/representation-action-gap.md|representation-action-gap]]
- [[entities/vector-quantization.md|vector-quantization]]
- [[entities/semantic-id-tokenization.md|semantic-id-tokenization]]
- [[entities/tokenization.md|tokenization]]
- [[entities/latent-aligned-planning.md|latent-aligned-planning]]
- [[entities/action-tokenization.md|action-tokenization]]

## 📐 개념

- [[concepts/latent-aligned-planning.md|latent-aligned-planning]]
- [[concepts/action-tokenization.md|action-tokenization]]
- [[concepts/discrete-continuous-adaptation-transition.md|discrete-continuous-adaptation-transition]]
- [[concepts/tokenization.md|tokenization]]
- [[concepts/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]

---
_LLM 분석으로 생성됨_
