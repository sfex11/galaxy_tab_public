# Discriminative World Models for Web Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02885v1

## 💡 핵심 인사이트

세계 모델의 진짜 품질 지표는 예측 상태의 재구성 춥실도가 아니라 하류 랭커·PRM이 후보 행동을 구별하는 데 필요한 판별성이며, 학습 목표를 이 판별적 용도에 정렬하는 것이 테스트타임 행동 선택 성능의 상한을 결정한다.

## 📖 분석

본 논문은 웹 에이전트의 테스트타임 행동 선택을 지탱하는 [[world-model]]의 학습 목표와 추론 용도 간 구조적 부정합을 진단한다. 기존 세계 모델은 HTML·AXTree 스냅샷 같은 고정 표현의 충실한 재구성을 목표로 하는 생성적 다음 상태 예측으로 훈련되지만, 실제 추론에서는 후보 행동들의 예측 상태를 process-reward-model이나 랭커로 비교·순위화하는 판별적 용도로 소비된다. 재구성 충실도는 후보 간 차별화 능력을 보장하지 않으므로, 학습이 상류 표현 아티팩트(스냅샷 재현)에 매몰되는 [[artifact-bound-optimization]] 패턴의 세계 모델 계층 사례가 된다. 논문의 해법인 판별적 훈련은 검증 기준이 정답 상태와의 절대 일치에서 후보 간 상대적 우열로 이동하는 [[relative-verifiability]] 전환과 동형이며, 상태 세부의 유용성이 내재 속성이 아니라 결정 과제에 대한 관계 속성임을 보여 [[utility-ontological-mislocation]]을 실증한다. 아울러 과제 조건화된 관련성 압축으로서 [[compression-relevance-isomorphism]]과 접속되고, 후보 샘플링→예측→순위화 파이프라인의 병목이 랭커가 아닌 상류 세계 모델의 판별성에 있음을 보여 [[test-time-scaling]]의 병목 지도를 갱신한다. 운전 도메인 생성적 세계 모델(VectorWorld, Fail2Drive)과 대비되어, 세계 모델의 과제별 특수화가 필연이라는 [[world-model-in-pieces]] 진단을 웹 도메인에서 재확인시킨다.

## 🔗 관련 논문

- VectorWorld: Efficient Streaming World Model via Diffusion
- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- ClawBench: Can AI Agents Complete Everyday Online Tasks?

## 🏷️ 엔티티

- [[entities/discriminative-world-model.md|discriminative-world-model]]

## 📐 개념

- [[concepts/world-model.md|world-model]]
- [[concepts/process-reward-model.md|process-reward-model]]
- [[concepts/artifact-bound-optimization.md|artifact-bound-optimization]]
- [[concepts/relative-verifiability.md|relative-verifiability]]
- [[concepts/utility-ontological-mislocation.md|utility-ontological-mislocation]]
- [[concepts/compression-relevance-isomorphism.md|compression-relevance-isomorphism]]
- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/generation-ranking-objective-misalignment.md|generation-ranking-objective-misalignment]]

---
_LLM 분석으로 생성됨_
