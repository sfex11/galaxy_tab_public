# CrossDepth: Geometry-Constrained Attention for Generalizable Multi-View Surround Depth Estimation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05397v1

## 💡 핵심 인사이트

인접 뷰의 중첩이 최소인 서라운드 리그에서 다중 뷰 깊이는 뷰 간 매칭이 아니라 단안 외관 단서의 교차 이미지 해석 일관성 위에 서 있으며, 이 일관성을 기하 제약으로 어텐션에 직접 주입하는 것이 일반화 가능한 깊이 추정의 핵심 조건이다.

## 📖 분석

# CrossDepth: Geometry-Constrained Attention for Generalizable Multi-View Surround Depth Estimation (2026-09-08)

## 핵심 기여

자율주행 서라운드 카메라 리그의 근본적 기하학적 조건을 문제화한다: 인접 카메라 이미지의 중첩이 최소화되어 대부분의 픽셀 깊이는 단안 외관 단서에 의존할 수밖에 없다. CrossDepth는 동일한 외관 단서가 이미지마다 다르게 해석되는 교차 이미지 불일치의 두 주요 원인을 정면으로 다루며, 어텐션 메커니즘에 기하 제약을 직접 주입하여 해결한다.

## Wiki 연결

- [[monocular-depth-estimation]] (CADENCE, 2026-04-10)이 '컨텍스트 적응적 깊이 추정'을 다뤘다면, 본 논문은 단안 깊이가 다중 뷰에서 상호 일관되도록 강제하는 '교차 뷰 일관성' 축을 추가한다. 단안 깊이가 독립 예측에서 교차 뷰 검증 대상으로 재정의된다.
- [[autonomous-driving-perception]]과 [[3d-scene-understanding]] 관점에서 LiDAR 융합([[lidar-camera-fusion]]) 없이 카메라만으로 3D 신뢰성을 확보하는 순수 비전 경로를 제시한다.
- 'Generalizable'이라는 목표는 [[generalization-gap]]에 센서 리그 구성 변화(카메라 개수·배치)에 대한 강건성이라는 새 하위 축을 제안한다.

## 새 개념

- **geometry-constrained-attention**: 관련성만으로 작동하는 어텐션에 3D 기하 사전(상대 포즈·에피폴라)을 구조적 제약으로 주입하는 패러다임.
- **cross-image-consistency**: 외관-깊이 매핑의 일관성이 매칭의 부산물이 아니라 일차 학습 목표가 되는 전환.

## 🔗 관련 논문

- CADENCE: Context-Adaptive Depth Estimation for Navigation an
- Toward Robust LiDAR Semantic Segmentation for Real-World Dep
- LEO: Graph Attention Network based Hybrid Multi Sensor Exten

## 🏷️ 엔티티

- [[entities/crossdepth.md|crossdepth]]
- [[entities/surround-depth-estimation.md|surround-depth-estimation]]
- [[entities/monocular-depth-estimation.md|monocular-depth-estimation]]
- [[entities/autonomous-driving-perception.md|autonomous-driving-perception]]
- [[entities/3d-scene-understanding.md|3d-scene-understanding]]
- [[entities/generalization-gap.md|generalization-gap]]

## 📐 개념

- [[concepts/geometry-constrained-attention.md|geometry-constrained-attention]]
- [[concepts/cross-image-consistency.md|cross-image-consistency]]
- [[concepts/generalizable-depth-estimation.md|generalizable-depth-estimation]]
- [[concepts/minimal-overlap-surround-view.md|minimal-overlap-surround-view]]

---
_LLM 분석으로 생성됨_
