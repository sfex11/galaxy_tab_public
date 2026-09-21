# PRIME: Perception Feedback with Situational Memory Embeddings in VLA Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22040v1

## 💡 핵심 인사이트

VLA 모델의 지각이 하류 추론·계획 목표에 맹목적인 것은 표현 형식의 문제가 아니라 정보 흐름의 단방향성 문제이며, 상황 기억 임베딩을 통한 학습된 피드백이 이 흐름을 양방향으로 전환한다.

## 📖 분석

PRIME는 자율주행 VLA 모델의 지각-추론-계획 위계가 피드포워드로만 작동할 때 초기 지각이 하류 추론·항행 목표를 모른 채 시각 입력을 무차별 처리하는 구조적 맹목성을 진단하고, 학습된 피드백 메커니즘으로 해소한다. 상황 기억 임베딩이 사전 결정을 지각 모듈로 되돌려, 지각이 목표 정보화된 큐 우선순위를 획득하게 한다.

기존 Wiki와의 세 연결점: 첫째, [[closed-loop-training]]의 폐루프를 환경-에이전트 경계가 아닌 에이전트 내부(계획→지각)로 이동시킨 에이전트 내부 폐루프 사례다. 둘째, [[plan-centric-steering]]이 유지된 계획이 상호작용을 재구성한다는 통찰을 지각 계층까지 구현하여, 계획이 행동 선택과 지각 우선순위를 함께 조향하는 위계를 완성한다. 셋째, [[thinking-acting-gap]]의 원인을 표현 형식 차이([[action-tokenization]])가 아닌 정보 흐름의 단방향성으로 재진단하는 별도 축을 제공한다.

[[latent-aligned-planning]] 계열 연구가 지각→행동 잠재 정렬을 다뤘다면 PRIME은 추론→지각의 역방향 정렬을 추가하여, VLA 정렬이 파이프라인 내 모든 인접 계층 쌍에 존재하는 문제임을 보여준다. [[render-free-teacher]] 경로의 온폴리시 운전 미세조정과 함께 자율주행 VLA 폐루프 훈련 연구군을 형성한다.

## 🔗 관련 논문

- OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia

## 🏷️ 엔티티

- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/autonomous-driving.md|autonomous-driving]]

## 📐 개념

- [[concepts/perception-feedback.md|perception-feedback]]
- [[concepts/situational-memory-embedding.md|situational-memory-embedding]]
- [[concepts/feedforward-hierarchy-blindness.md|feedforward-hierarchy-blindness]]
- [[concepts/thinking-acting-gap.md|thinking-acting-gap]]
- [[concepts/closed-loop-training.md|closed-loop-training]]
- [[concepts/plan-centric-steering.md|plan-centric-steering]]
- [[concepts/latent-aligned-planning.md|latent-aligned-planning]]
- [[concepts/render-free-teacher.md|render-free-teacher]]

---
_LLM 분석으로 생성됨_
