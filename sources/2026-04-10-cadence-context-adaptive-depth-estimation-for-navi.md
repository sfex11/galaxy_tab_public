# CADENCE: Context-Adaptive Depth Estimation for Navigation and Computational Efficiency

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-10
**링크**: http://arxiv.org/abs/2604.07286v1

## 💡 핵심 인사이트

장면 맥락에 따라 깊이 추정 네트워크의 연산 복잡도를 동적으로 조절함으로써, 자원 제약 환경에서 정확도와 효율성의 실시간 트레이드오프를 달성한다.

## 📖 분석

## CADENCE: Context-Adaptive Depth Estimation for Navigation and Computational Efficiency

자율주행 차량이 원격 환경에서 제한된 임베디드 프로세서, 소형 배터리, 경량 센서로 운용될 때 발생하는 연산 제약 문제를 해결하기 위한 적응형 시스템이다. CADENCE는 **slimmable monocular depth estimation 네트워크**의 연산 복잡도를 동적으로 조절하여, 장면의 맥락(context)에 따라 정확도와 효율성 사이의 트레이드오프를 실시간으로 최적화한다.

### 기존 Wiki와의 관계

이 연구는 [[concepts/autonomous-driving.md|autonomous driving]]과 [[concepts/on-device-inference.md|on device inference]] 개념의 교차점에 위치한다. 제한된 하드웨어에서 깊이 추정 모델을 효율적으로 실행한다는 점에서, 에너지-성능 트레이드오프를 다룬 *Sustainability Is Not Linear* 연구와 직접적으로 맥을 같이 한다. 또한 [[concepts/sensor-fusion.md|sensor fusion]] 관점에서 단안(monocular) 카메라만으로 깊이를 추정한다는 점은 LiDAR-카메라 융합 기반의 *Deep Neural Network Based Roadwork Detection* 접근과 대조적이다.

**Slimmable network** 기법은 [[concepts/model-pruning.md|model pruning]]과 [[concepts/model-compression.md|model compression]]의 연장선상에 있으며, 단일 모델 내에서 폭(width)을 동적으로 조절하여 여러 정확도-비용 운영점을 제공한다. 이는 정적 프루닝과 달리 런타임에 적응이 가능하다는 점에서 차별화된다.

### 핵심 기여

장면 복잡도에 따라 네트워크 용량을 자동 조절하는 **context-adaptive 스케줄링**은 단순한 모델 경량화를 넘어, 환경 인식 기반의 연산 자원 할당이라는 새로운 패러다임을 제시한다. 이는 로보틱스와 엣지 AI 전반에 적용 가능한 설계 원칙이다.

## 🔗 관련 논문

- Deep Neural Network Based Roadwork Detection for Autonomous Driving
- Sustainability Is Not Linear: Quantifying Performance, Energy
- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- Cram Less to Fit More: Training Data Pruning Improves Memorization

## 📐 개념

- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/monocular-depth-estimation.md|monocular-depth-estimation]]
- [[concepts/slimmable-network.md|slimmable-network]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/monocular-pose-estimation.md|monocular pose estimation]]

---
**관련**: [[concepts/collaboration-depth-axis.md|collaboration depth axis]]
