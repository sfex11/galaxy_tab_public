# OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Free Teacher

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20756v1

## 💡 핵심 인사이트

렌더링 프리 교사는 폐루프 훈련이 환경 시뮬레이션 없이도 교사 판단 신호만으로 성립할 수 있음을 보여주며, 환경 공급 병목에 대한 '환경 없는 폐루프'라는 제3의 해법 경로를 연다.

## 📖 분석

OPTED는 자율주행 end-to-end 정책의 오픈루프 행동 복제 사전학습이 폐루프 배포에서 오류 누적(compounding error)을 일으켜 차량을 훈련 분포 밖으로 유도한다는 문제를 진단하고, 온폴리시 파인튜닝으로 이를 교정하되 렌더링 프리 교사(render-free teacher)로 폐루프 훈련의 시뮬레이션 비용을 제거한다.

## 기존 Wiki와의 관계

- [[closed-loop-training]]: '폐루프는 어떻게 환경을 공급받는가'라는 질문에 제3의 답을 제공한다. 궤적 재활용이나 환경 진화가 환경 자체를 공급했다면, OPTED는 환경 렌더링 없이 교사의 판단 신호만으로 루프를 닫는 '환경 없는 폐루프' 경로를 연다. 이는 [[environment-absence-bottleneck]]에 대한 역설적 해법이다.
- [[compounding-error]]: 회복 불가능한 오류의 자율주행 도메인 발현을 제공하며, 오프폴리시 사전학습 → 폐루프 배포의 인과 경로를 입증한다.
- [[on-policy-distillation]]: 온폴리시 정정의 목적을 약한 모델 따라잡기에서 분포 이탈 방지(안전)로 확장하며, 물리 도메인에서의 유효성을 입증한다.
- [[model-based-rl]]: 세계 모델링 없이 교사가 환경 시뮬레이션의 판단 기능만 대체하는 경량 경로를 제시한다.
- [[end-to-end-vla-training]]: 행동 복제 기준선의 구조적 한계를 진단하고 같은 파이프라인 안에 폐루프 파인튜닝 계층을 추가한다.

physical AI에서 사후학습의 위상이 효율 최적화에서 안전 보장으로 이동하는 흐름([[post-training]])을 자율주행으로 확장한다.

## 🔗 관련 논문

- A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia
- Continuous Actions from Discrete Minds: Latent-Aligned Plann
- Learning Agent-based Model Predictive Control for Holistic V
- Environment Evolution for Terminal Agents
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E

## 🏷️ 엔티티

- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/post-training.md|post-training]]
- [[entities/closed-loop-training.md|closed-loop-training]]
- [[entities/model-based-rl.md|model-based-rl]]
- [[entities/on-policy-distillation.md|on-policy-distillation]]
- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]
- [[entities/distribution-shift.md|distribution-shift]]

## 📐 개념

- [[concepts/render-free-teacher.md|render-free-teacher]]
- [[concepts/compounding-error.md|compounding-error]]
- [[concepts/self-induced-distribution-shift.md|self-induced-distribution-shift]]

---
_LLM 분석으로 생성됨_
