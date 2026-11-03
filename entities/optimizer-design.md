# optimizer-design

**카테고리**: 미분류
**생성일**: 2026-10-30

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-10-30-muongs-pretraining-llms-with-relaxed-weight-norm-c.md|MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control]]

### Pretraining Data Scale Reverses the Muon-AdamW Fine-Tuning Gap (2026-11-04)

MuonGS가 norm control의 이론적 통일(C_T 상한)을 제시한 데 이어, 본 논문은 옵티마이저 선택(Muon vs AdamW)의 우위가 사전학습 손실에서는 성립하지만 데이터 규모가 충분히 크면 파인튜닝 후 하류 성능에서 역전함을 실증한다. 옵티마이저의 효과 평가가 사전학습 시점 단일 지표를 넘어 사후학습 파이프라인 종단 성능으로 확장되어야 함을 보여준다.

→ [[sources/2026-11-04-pretraining-data-scale-reverses-the-muon-adamw-fin.md|상세 보기]]
