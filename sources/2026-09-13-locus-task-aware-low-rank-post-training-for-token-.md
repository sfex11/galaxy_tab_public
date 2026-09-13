# LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-13
**링크**: http://arxiv.org/abs/2609.11739v1

## 💡 핵심 인사이트

정렬 손실을 전혀 수정하지 않고 업데이트가 위치할 저계수 부공간의 태스크 인지적 선택만으로 출력 토큰 비용을 제어할 수 있으며, 이는 품질 목표와 비용 목표가 별도의 파라미터 축으로 분해 가능함을 실증한다.

## 📖 분석

LOCUS는 사후학습 업데이트의 매개변수화 자체가 출력 길이를 결정하는 독립 제어 축임을 실증한다 — 정렬 손실을 전혀 수정하지 않고 업데이트 부공간(저계수 적응 공간)의 태스크 인지적 선택만으로 토큰 비용을 최소화하되 유틸리티 제약을 유지한다. 본 논문은 2026-09-12에 이미 수록되어 있으므로 이 항목은 기존 분석의 심화판이다.

훈련 시점 축 추가: [[concepts/parameter-decoupling.md|parameter decoupling]] 논의에서 이산 확산의 샘플러 교체([[concepts/distribution-preserving-acceleration.md|distribution preserving acceleration]])가 추론 시점의 분포-절차 분리였다면, 본 논문은 품질 목표(정렬 손실)와 비용 목표(시퀀스 길이)가 업데이트 파라미터의 위치에서 분해됨을 보여준다. [[concepts/length-inflation.md|length inflation]]과의 관계도 재정의된다 — OPD의 길이 부풀림이 억제 대상 병리였다면 LOCUS는 길이를 양방향 조정 가능한 출력 차원으로 격상시킨다. preference alignment의 장황화([[concepts/reward-hacking.md|reward hacking]]의 온건한 발현)에 보상 재설계가 아닌 부공간 제약으로 응답하는 구조적 경로를 제공하며, [[concepts/cost-dominance-dimension-asymmetry.md|cost dominance dimension asymmetry]]의 행동 축(토큰 소비) 제어점을 추론 최적화 이전 사후학습 단계로 이동시킨다. '어디에 업데이트할 것인가'의 국소화는 [[entities/layer-selective-unlearning.md|layer selective unlearning]]의 '어디를 잊을 것인가'와 병렬되는 매개변수 공간 국소화 패턴을 형성한다.

## 🔗 관련 논문

- LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Generation (2026-09-12, 기존 수록본)
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion (2026-09-07)
- Crafting Reversible SFT Behaviors in Large Language Models (2026-05-10)
- Demystifying OPD: Length Inflation and Stabilization Strategies (2026-04-12)

## 🏷️ 엔티티

- [[entities/task-aware-subspace-selection.md|task-aware-subspace-selection]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/length-inflation.md|length-inflation]]
- [[entities/cost-dominance-dimension-asymmetry.md|cost-dominance-dimension-asymmetry]]
- [[entities/low-rank-adaptation-subspace.md|low-rank-adaptation-subspace]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[entities/post-training.md|post-training]]
- [[entities/reward-hacking.md|reward-hacking]]

## 📐 개념

- [[concepts/parameter-decoupling.md|parameter-decoupling]]
- [[concepts/low-rank-adaptation-subspace.md|low-rank-adaptation-subspace]]
- [[concepts/length-inflation.md|length-inflation]]
- [[concepts/cost-dominance-dimension-asymmetry.md|cost-dominance-dimension-asymmetry]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[concepts/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[concepts/reward-hacking.md|reward-hacking]]

---
_LLM 분석으로 생성됨_
