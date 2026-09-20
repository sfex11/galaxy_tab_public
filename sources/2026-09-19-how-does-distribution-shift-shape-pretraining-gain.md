# How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20814v1

## 💡 핵심 인사이트

사전학습의 전이 이득은 분포 시프트의 어느 성분이 변하는가(기하 vs 물리 모델링)에 따라 이질적으로 나타나므로, 시프트의 성분 분해가 전이 이득 예측의 선행 조건이 된다.

## 📖 분석

### How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates? (2026-09-19)

한 에어포일 계열의 254,909개 RANS 해로 사전학습한 신경망 PDE 서로게이트가 기하·물리 변화 시 새로운 CFD 데이터 필요량을 얼마나 줄이는지 정량 분석한다. 자유류 범위를 통제한 두 타깃 설정(동일 SA 모델링 vs SA+e^N 전이 모델링 추가)으로 미세조정하여 시프트 성분을 격리하는 실험 설계를 채택한다.

[[concepts/transfer-learning.md|transfer learning]]에 과학 컴퓨팅 도메인의 사례를 추가한다 — Wiki의 전이 학습 논의가 LLM 중심이었던 것과 달리, 물리 시뮬레이션에서도 전이 이득이 시프트의 성격에 조건부임을 실증하며 [[entities/scale-conditional-training-strategy.md|scale conditional training strategy]]와 동형의 조건부 유효성 구조를 형성한다. [[entities/auxiliary-views.md|auxiliary views]] 계열과 함께 '사전학습이 언제 이득인가'라는 질문의 도메인 확장이다.

[[concepts/distribution-shift.md|distribution shift]]에 분석적 기여를 제공한다. 시프트를 단일 변인으로 다루던 기존 논의와 달리 기하 시프트와 물리 모델링 시프트로 분해하여 어느 성분이 사전학습 이득을 결정하는지 통제 실험으로 격리한다. 자유류 범위 매칭 설계는 [[entities/preregistered-measurement-audit.md|preregistered measurement audit]]의 통제된 측정 전통과 정합되며, 시프트의 성분 분해가 전이 이득 예측의 선행 조건임을 시사한다.

## 🔗 관련 논문

- Knowledge Acquisition During Pre-training? Large Language Models Learn
- Multi-Agent Reinforcement Learning for Autonomous UAV Explor
- Post-Training Language Models for Gold-Medal Performance in 

## 🏷️ 엔티티

- [[entities/transfer-learning.md|transfer-learning]]
- [[entities/distribution-shift.md|distribution-shift]]
- [[entities/neural-pde-surrogate.md|neural-pde-surrogate]]
- [[entities/shift-component-decomposition.md|shift-component-decomposition]]

## 📐 개념

- [[concepts/shift-component-decomposition.md|shift-component-decomposition]]
- [[concepts/data-efficiency-gains-from-pretraining.md|data-efficiency-gains-from-pretraining]]
- [[concepts/matched-condition-comparison.md|matched-condition-comparison]]

---
_LLM 분석으로 생성됨_
