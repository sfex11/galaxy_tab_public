# Deep Neural Network Based Roadwork Detection for Autonomous Driving

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-06
**링크**: http://arxiv.org/abs/2604.02282v1

## 💡 핵심 인사이트

도로 공사 현장이라는 극도로 동적이고 이질적인 환경에서 YOLO+LiDAR 융합을 통해 개별 객체 탐지를 넘어 coherent한 공사 구역 수준의 이해를 달성한 점이, 자율주행 perception의 실용적 도전 과제를 잘 보여준다.

## 📖 분석

## Deep Neural Network Based Roadwork Detection for Autonomous Driving

본 논문은 자율주행 차량을 위한 실시간 도로 공사 현장 탐지 시스템을 제안한다. YOLO 신경망과 LiDAR 데이터를 결합하여 주행 중 개별 도로 공사 객체를 식별하고, 이를 일관된 공사 현장으로 병합한 뒤 월드 좌표계에서 윤곽을 기록하는 파이프라인을 구성한다.

### 핵심 접근법
- **YOLO 기반 객체 탐지**: 도로 공사 관련 객체(콘, 바리케이드, 표지판 등)를 실시간으로 검출
- **LiDAR 융합**: 카메라 기반 탐지 결과에 LiDAR 포인트 클라우드를 결합하여 3D 위치 추정 및 월드 좌표 변환 수행
- **공간 클러스터링**: 개별 객체를 시공간적으로 병합하여 coherent한 공사 구역으로 그룹화
- **미국 데이터셋 적응**: 기존 US 데이터셋을 적응(adapt)하고 새로운 데이터셋을 구축하여 모델 학습에 활용

### Wiki 내 위치
본 연구는 [[autonomous-driving]] 분야의 인식(perception) 파이프라인에 해당하며, 특히 [[autonomous-driving-perception]]의 센서 융합 접근과 직접적으로 연결된다. 기존 Wiki의 AdaRadar가 레이더 기반 스펙트럼 압축을 다뤘다면, 본 논문은 카메라+LiDAR 융합으로 도로 공사라는 특수 시나리오에 초점을 맞춘다. 또한 [[distribution-shift]] 관점에서, 도로 공사 현장은 일반 주행 환경과 크게 다른 동적 환경을 형성하므로 자율주행 모델의 일반화 능력을 시험하는 중요한 테스트 케이스다. Fail2Drive 벤치마크가 제기한 closed-loop 일반화 문제와도 맥을 같이한다.

## 🔗 관련 논문

- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- AdaRadar: Rate Adaptive Spectral Compression for Radar-based
- VectorWorld: Efficient Streaming World Model via Diffusion F
- CADENCE: Context-Adaptive Depth Estimation for Navigation

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/autonomous-driving-perception.md|autonomous-driving-perception]]
- [[concepts/object-detection.md|object-detection]]
- [[concepts/lidar-camera-fusion.md|lidar-camera-fusion]]
- [[concepts/distribution-shift.md|distribution-shift]]

---
_LLM 분석으로 재생성됨_
