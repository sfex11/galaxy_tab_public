# parallel-decoding

**카테고리**: 미분류
**생성일**: 2026-05-01

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-01-turning-the-tide-cross-architecture-distillation-f.md|Turning the TIDE: Cross-Architecture Distillation for Diffus]]

### Continuous Latent Diffusion Language Model (2026-05-10)

Cola DLM은 병렬 디코딩의 적용 대상을 자회귀 생성 내부(추측 디코딩, SpecKV 등)에서 패러다임 외부(확산 기반 비순차 생성)로 확장한다. 기존 병렬 디코딩이 타겟 분포 무변경 원칙 하에서 수용률을 최적화했다면, Cola DLM은 분포 자체를 비순차적으로 재설계하여 병렬화의 구조적 제약을 원천적으로 제거한다.

### Visual-Redundancy-Controlled Parallel Decoding for Diffusion-Based Mul (2026-05-27)

### Visual-Redundancy-Controlled Parallel Decoding for Diffusion-Based Multimodal LLMs (2026-05-27)
기존 신뢰도 기반 병렬 디코딩이 타겟 분포 무변경 원칙 하에서만 각 마스크 위치의 신뢰도를 독립적으로 순위하여 상위-K를 커밋하는 한계를 식별한다. dMLLM의 비순차 생성 특성(시각 토큰의 지역적 연관성)을 고려하여, 위치 간 상호 연관성이 높은 그룹을 단위로 커밋하는 **위치 간 중복성 제어**를 도입한다. 이는 자회귀 접근이 불필요한 연산을 낭비하는 동시에, 독립적 순위만으로는 불충분한 컨텍스트를 생성하는 기존 접근의 구조적 한계를 해소한다.

### Unlocking Lossless Speedups in LLMs via Discrete Diffusion (2026-09-06)

병렬 디코딩의 적용 방식에 'AR 분포로부터의 확산 기반 직접 샘플링'이라는 새 경로를 추가한다. 분포 재설계(Cola DLM)와 수용률 최적화(추측 디코딩) 사이의 중간 지점을 채운다.

### Discrete Beckmann Transport Models for One-Step Language Modeling and  (2026-09-16)

비순차 생성의 실현 경로에 '동역학계 고정점으로의 수렴'을 추가한다. 스텝 수를 외부 하이퍼파라미터가 아닌 자율 사상의 반복 적용으로 결정하는 구조는 병렬 디코딩의 스텝-품질 딜레마에 대한 새로운 접근이다.

→ [[sources/2026-09-16-discrete-beckmann-transport-models-for-one-step-la.md|상세 보기]]

### Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruning (2026-09-18)

병렬화(얼마나 동시에 생성하는가)와 선택(어떤 후보를 남길 것인가)이 직교하는 최적화 축임을 명확히 한다. 순차 디코딩 내부의 선택 계층 개선이 병렬화 논의와 독립적으로 성립하는 사례를 제공한다.

→ [[sources/2026-09-18-beyond-truncation-rethinking-llm-decoding-as-ensem.md|상세 보기]]
