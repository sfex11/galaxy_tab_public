# Beyond Truncation: Rethinking LLM Decoding as Ensemble Pruning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.18723v1

## 💡 핵심 인사이트

후보 토큰 선택을 확률 순위 매기기가 아닌 기하학적 앙상블 가지치기로 재정의하면, 훈련이나 복잡한 재가중 없이도 스칼라 확률이 소실시키는 후보 간 의미적 중복 정보를 회복할 수 있다.

## 📖 분석

ME-Decoding(Mahalanobis-Ensemble Decoding)은 후보 토큰 선택을 앙상블 가지치기로 재정의하는 디코딩 프레임워크다. top-k·nucleus 등 기존 선택이 스칼라 확률에만 의존하여 후보 간 기하학적 의미 관계를 무시하고 중복 후보를 낳는다는 진단에서 출발하며, 마할라노비스 거리로 후보 임베딩의 공분산 구조를 반영해 중복을 제거한다. 이는 [[output-space-pruning]]의 확장이다 — TeCoD가 외부 도메인 템플릿으로 출력 공간을 축소했다면, 본 논문은 모델 내부 표현의 기하학이라는 내부 근거로 후보를 가지치기하여 프루닝 근거의 위치를 도메인 지식에서 표현 공간으로 이동시킨다. [[local-sufficiency]]의 Select to Think가 토큰 선택 전략만으로 품질을 높였듯, 본 논문은 재가중이나 복잡한 최적화 없이 선택 개선이 가능한 training-free 경로를 강화한다. [[distribution-preserving-acceleration]] 계열(추측 디코딩, 이산 확산 샘플러)이 분포 보존 아래 가속을 추구한다면, 본 논문은 분포 변경을 수용하고 선택 품질 자체를 목표로 하는 제3의 디코딩 최적화 축을 제시한다. [[marginal-distribution-ceiling]] 관점에서 스칼라 확률 순위는 P(y)의 판독일 뿐 후보 간 조건부 중복 구조를 담지 못하므로, P(y)를 바꾸지 않고도 [[parallel-decoding]]과 직교하는 선택 계층 개선이 가능함을 보여준다.

## 🔗 관련 논문

- Reliable Answers for Recurring Questions: Boosting Text-to-SQL Accurac
- Select to Think: Unlocking SLM Potential with Local Sufficie
- Unlocking Lossless Speedups in LLMs via Discrete D

## 🏷️ 엔티티

- [[entities/mahalanobis-ensemble-decoding.md|mahalanobis-ensemble-decoding]]
- [[entities/output-space-pruning.md|output-space-pruning]]
- [[entities/local-sufficiency.md|local-sufficiency]]
- [[entities/distribution-preserving-acceleration.md|distribution-preserving-acceleration]]
- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/parallel-decoding.md|parallel-decoding]]

## 📐 개념

- [[concepts/ensemble-pruning-decoding.md|ensemble-pruning-decoding]]
- [[concepts/candidate-semantic-redundancy.md|candidate-semantic-redundancy]]
- [[concepts/scalar-probability-selection-insufficiency.md|scalar-probability-selection-insufficiency]]
- [[concepts/geometric-selection-criterion.md|geometric-selection-criterion]]

---
_LLM 분석으로 생성됨_
