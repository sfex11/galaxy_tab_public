# parameter-decoupling

**카테고리**: 미분류
**생성일**: 2026-09-07

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-07-unlocking-lossless-speedups-in-llms-via-discrete-d.md|Unlocking Lossless Speedups in LLMs via Discrete Diffusion]]

### LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language  (2026-09-12)

파라미터화-행동 분리의 새 축을 제공한다. 기존에는 샘플러 교체(이산 확산으로 분포 유지 병렬화)가 이 분리의 사례였다면, 본 논문은 정렬 손실 불변 하에서 업데이트 부공간이 시퀀스 길이를 조정함을 보여, 품질 목표와 비용 목표가 별도 파라미터 축으로 분해 가능함을 확장한다.

### LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language  (2026-09-13)

정렬 손실 불변 하에서 업데이트 부공간이 시퀀스 길이를 조절함을 보여, 품질 목표와 비용 목표의 분해가 추론 시점(샘플러 교체)을 넘어 사후학습 업데이트의 매개변수화 수준에서도 성립함을 확장한다.

### Learning to Coach for Experiential Learning (2026-09-16)

분리의 새 축을 추가한다 — 품질-비용 분리(LOCUS), 분포-샘플러 분리(이산 확산)에 이어 '성능 파라미터(액터)-개선 파라미터(코치)'의 모듈 간 분리를 제시한다. 개선이 액터 파라미터를 건드리지 않고 별도 공간에서 진행 가능함을 실증한다.

### Merging the Knowledge of LLMs for Automatic Speech Recognition (2026-09-16)

지식 통합의 시점 축을 추가한다. LOCUS가 품질-비용을 별도 파라미터 축으로 분해했다면, 본 논문은 외부 LM 지식을 추론 시 매개할지 파라미터에 사전 흡수할지의 선택 자체가 파라미터화 결정임을 보여준다.
