# Better than Average: Spatially-Aware Aggregation of Segmentation Uncertainty Improves Downstream Performance

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-02
**링크**: http://arxiv.org/abs/2603.29941v1

## 💡 핵심 인사이트

세그멘테이션 불확실성의 공간적 분포를 고려한 집계 전략이 단순 평균 대비 OoD 탐지 및 실패 감지 성능을 유의미하게 향상시킨다.

## 📖 분석

## Better than Average: Spatially-Aware Aggregation of Segmentation Uncertainty Improves Downstream Performance

### 개요
본 논문은 이미지 세그멘테이션에서 생성된 픽셀 단위 불확실성 점수를 이미지 수준 점수로 집계(aggregation)하는 전략의 특성과 하류 작업 성능에 대한 영향을 체계적으로 분석한다. 생의학 이미지 분석이나 자율주행과 같은 안전 필수 도메인에서 불확실성 정량화(UQ)는 자동화된 세그멘테이션의 신뢰성 확보에 핵심적이다.

### 핵심 기여
기존에는 픽셀별 불확실성을 단순 평균(mean)으로 집계하는 방식이 관행적으로 사용되었으나, 본 연구는 이 접근이 최적이 아님을 보여준다. **공간 인식 집계(spatially-aware aggregation)** 전략을 제안하여, 불확실성의 공간적 분포 패턴을 고려함으로써 OoD(Out-of-Distribution) 탐지 및 실패 감지(failure detection)와 같은 하류 작업에서 성능을 개선한다.

### 기존 연구와의 연결
본 논문의 불확실성 정량화 접근법은 [[uncertainty-quantification]] 개념과 직접적으로 관련된다. Semantic Token Clustering 연구가 토큰 수준에서 효율적 UQ를 다뤘다면, 본 연구는 세그멘테이션 도메인에서 집계 전략이라는 상보적 측면을 탐구한다. 또한 자율주행 인식([[autonomous-driving-perception]], [[autonomous-driving]])의 안전성 확보와 밀접하며, OoD 탐지 관점에서 [[distribution-shift]] 문제와도 연결된다. 공간 정보 활용이라는 측면에서 [[spatial-reasoning]] 개념과의 접점도 존재한다.

## 🔗 관련 논문

- Semantic Token Clustering for Efficient Uncertainty Quantifi
- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- AdaRadar: Rate Adaptive Spectral Compression for Radar-based

## 📐 개념

- [[concepts/uncertainty-quantification.md|uncertainty-quantification]]
- [[concepts/autonomous-driving-perception.md|autonomous-driving-perception]]
- [[concepts/spatial-reasoning.md|spatial-reasoning]]
- [[concepts/distribution-shift.md|distribution-shift]]

---
_LLM 분석으로 재생성됨_
