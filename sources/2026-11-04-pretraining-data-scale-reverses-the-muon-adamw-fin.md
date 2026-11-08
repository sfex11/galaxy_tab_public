# Pretraining Data Scale Reverses the Muon-AdamW Fine-Tuning Gap

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03633v1

## 💡 핵심 인사이트

사전학습 옵티마이저의 우위는 데이터 규모와 모델 크기에 따라 하류 파인튜닝 성능에서 역전될 수 있으며, 옵티마이저의 가치 평가는 사전학습 손실이 아닌 종단 파이프라인 성능으로 이루어져야 한다.

## 📖 분석

## Pretraining Data Scale Reverses the Muon-AdamW Fine-Tuning Gap (2026-11-04)

**arXiv**: http://arxiv.org/abs/2611.03633v1

Muon이 사전학습에서 AdamW 대비 손실 최소화 속도 우위를 보이는 것과 달리, 충분히 큰 사전학습 데이터 예산을 넘어서면 파인튜닝 후 하류 성능은 AdamW가 역전하며, 모델 크기가 커질수록 역전 지점이 더 작은 데이터 규모에서 나타난다는 발견.

### Wiki 내 기존 논의와의 관계

**[[concepts/optimizer-design.md|optimizer design]] 확장**: MuonGS(2026-10-30)가 norm control을 누적 유효 학습률 C_T 상한으로 환원하며 옵티마이저 설계의 이론적 기반을 다졌다면, 본 논문은 사전학습 단계의 옵티마이저 선택이 하류 파인튜닝 성능에 비대칭적·역전적 영향을 미침을 실증하여 옵티마이저의 효과 평가가 사전학습 손실을 넘어 사후학습 파이프라인 전체로 확장되어야 함을 보여준다. Muon과 AdamW의 비교는 norm control 연구의 자연스러운 후속 검증 대상이다.

**[[concepts/data-efficiency-gains-from-pretraining.md|data efficiency gains from pretraining]] 심화**: PDE 서러게이트와 사전학습 이득 연구 계열이 '사전학습이 언제 도움이 되는가'를 다뤘다면, 본 논문은 사전학습 데이터 규모가 사전학습 시점 지표(손실)와 하류 시점 지표(파인튜닝 후 성능) 사이의 관계를 반전시킬 수 있음을 보여준다. 사전학습의 가치 평가가 단일 시점이 아닌 다단계 파이프라인의 속성임을 강화한다.

**[[concepts/scaling-laws.md|scaling laws]]와의 연결**: 'What do Language Models Learn and When?' 계열이 암묵적 커리큘럼과 스케일링을 다룬 흐름에, 데이터 규모×옵티마이저×모델 크기의 삼원 상호작용이라는 새 차원을 추가한다. 스케일링 법칙의 적용 대상이 데이터 양을 넘어 옵티마이저 선택으로 확장됨을 시사한다.

### 핵심 시사점

사전학습에서의 최적화 우위가 배포 파이프라인에서 유지되지 않을 수 있다는 것은, 훈련 파이프라인의 각 단계를 독립적으로 최적화하는 관행에 대한 교정이다. Wiki에서 반복 관찰된 [[concepts/training-inference-mismatch.md|training inference mismatch]], [[concepts/optimizer-model-consistency.md|optimizer model consistency]] 계열의 '단계 간 결합' 문제가 옵티마이저 선택 수준에서도 성립함을 확장한다. 옵티마이저의 가치를 사전학습 손실 곡선이 아닌 종단 성능으로 평가하는 패러다임 전환을 요구한다.

## 🔗 관련 논문

- MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control
- How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogate
- What do Language Models Learn and When? The Implicit Curriculum

## 🏷️ 엔티티

- [[entities/optimizer-design.md|optimizer-design]]
- [[entities/data-efficiency-gains-from-pretraining.md|data-efficiency-gains-from-pretraining]]
- [[entities/scaling-laws.md|scaling-laws]]
- [[entities/training-inference-mismatch.md|training-inference-mismatch]]

## 📐 개념

- [[concepts/pretraining-finetuning-gap-reversal.md|pretraining-finetuning-gap-reversal]]
- [[concepts/optimizer-dependent-scaling-crossover.md|optimizer-dependent-scaling-crossover]]
- [[concepts/downstream-inversion-of-pretraining-advantage.md|downstream-inversion-of-pretraining-advantage]]

---
_LLM 분석으로 생성됨_
