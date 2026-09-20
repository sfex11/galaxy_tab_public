# OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Free Teacher

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20756v1

## 💡 핵심 인사이트

정책 자신의 오류 누적이 만드는 자기유발 분포 이동은 언어 에이전트와 자율주행이 공유하는 도메인 불변 문제이며, 렌더 프리 교사는 폐루포스트트레이닝의 환경 렌더링 비용을 제거하여 물리 AI에서도 온폴리시 정정을 실용화한다.

## 📖 분석

# OPTED: 렌더 프리 교사를 통한 종단간 주행의 온폴리시 파인튜닝

## 핵심 주장
행동 클로닝(BC) 개루프 사전학습만으로 훈련된 종단간 주행 정책은 폐루프 배포에서 오류 누적(compounding error)로 스스로 훈련 분포 밖으로 이탈한다. OPTED는 폐루포스트트레이닝으로 이를 완화하되, 실제 세계 렌더링 없이 온폴리시 상태에서 교사 신호를 얻는 렌더 프리 교사로 폐루프 훈련의 비용 장벽을 제거한다.

## 위키 내 위치
- [[compounding-error]]의 인과 구조 입증 — LLM 에이전트의 다단계 도구 호출과 동일한 '정책의 과거 행동이 현재 입력 분포를 오염' 구조가 자율주행에서 재현되며, [[self-induced-distribution-shift]]의 도메인 불변성을 강화한다. UAV 야생화재([[non-stationary-dynamics]])의 외생적 이동과 대비되는 내생적 이동 사례다.
- [[on-policy-distillation]] 스펙트럼의 물리 극점 — 같은 시기의 언어 측 연구들([[retireopd]] 자가 퇴직 증류, [[score-centering]] 오프폴리시 안정화)과 병렬로, 온폴리시 신호의 용도가 능력 격차 해소에서 분포 이탈 방지·안전 완화로 확장됨을 보여준다.
- [[render-free-teacher]] — 교사가 세계 렌더링을 대체하는 것은 생성적 롤아웃을 판별적 평가로 치환하는 [[discriminative-world-model]] 경로의 운영 실현이며, [[imagination-relocation-to-training]]의 물리 버전이다.
- [[closed-loop-training]] — Terminal-Universe가 환경 공급으로 루프를 닫았다면, OPTED는 교사 신호로 루프를 닫는 제2 경로를 제시한다.
- [[post-training]] — '사전학습 확장의 한계 수익' 전제가 언어에서 물리 AI로 이식되어, 포스트트레이닝이 에이전트 계열의 공통 단계로 일반화 중임을 확인시킨다.
- [[end-to-end-vla-training]] — 미니어처 플랫폼([[miniature-vehicle-research-platform]])의 BC 기준선 위에 놓이는 폐루프 개선 계층을 제공한다.

## 🔗 관련 논문

- OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Free Teacher
- Score Centering Stabilizes Off-policy Reinforcement Learning
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments
- A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Miniature Vehicle
- How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates

## 🏷️ 엔티티

- [[entities/compounding-error.md|compounding-error]]
- [[entities/self-induced-distribution-shift.md|self-induced-distribution-shift]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/render-free-teacher.md|render-free-teacher]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/distribution-shift.md|distribution-shift]]
- [[entities/post-training.md|post-training]]
- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/non-stationary-dynamics.md|non-stationary-dynamics]]

## 📐 개념

- [[concepts/render-free-teacher.md|render-free-teacher]]
- [[concepts/self-induced-distribution-shift.md|self-induced-distribution-shift]]
- [[concepts/on-policyness-as-infrastructure-guarantee.md|on-policyness-as-infrastructure-guarantee]]
- [[concepts/closed-loop-training.md|closed-loop-training]]

---
_LLM 분석으로 생성됨_
