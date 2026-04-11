# LEO: Graph Attention Network based Hybrid Multi Sensor Extended Object Fusion and Tracking for Autonomous Driving Applications

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-03
**링크**: http://arxiv.org/abs/2604.02206v1

## 💡 핵심 인사이트

Graph Attention Network을 활용한 시공간 센서 융합으로 베이지안 확장 객체 모델의 이론적 견고성과 딥러닝의 적응성을 동시에 확보하여, 자율주행 객체 추적의 정확도와 효율성 트레이드오프를 개선했다.

## 📖 분석

## LEO: Graph Attention Network 기반 하이브리드 멀티센서 확장 객체 융합 및 추적

LEO(Learned Extension of Objects)는 자율주행에서 동적 객체의 정확한 형상 및 궤적 추정을 위해 고전적 베이지안 확장 객체 모델과 딥러닝을 결합한 하이브리드 접근법이다. 핵심 아키텍처로 시공간 Graph Attention Network(GAT)를 사용하여 멀티모달 센서 데이터(LiDAR, 카메라, 레이더 등)를 융합한다.

### 핵심 기여

기존 베이지안 확장 객체 모델은 사전 분포와 업데이트 우도 함수의 완전성에 의존하는 한계가 있고, 딥러닝 방식은 밀집 어노테이션과 높은 연산 비용이 문제였다. LEO는 두 패러다임의 장점을 결합하여, GAT의 어텐션 메커니즘으로 센서 간 관계를 동적으로 학습하면서도 베이지안 프레임워크의 이론적 견고성을 유지한다.

### Wiki 연결점

이 연구는 기존 Wiki의 여러 축과 교차한다. [[autonomous-driving]] 및 [[autonomous-driving-perception]] 개념과 직접적으로 연결되며, 레이더 인식을 다룬 AdaRadar 연구([[radar-perception]])와 센서 데이터 처리 관점에서 상보적이다. Graph Attention Network 구조는 [[transformer]] 엔티티의 어텐션 메커니즘 확장으로 볼 수 있으며, 멀티모달 센서 융합은 [[multimodal-learning]]의 인식 도메인 적용 사례이다. 또한 궤적 예측 측면에서 [[trajectory-prediction]], 센서 데이터 압축 측면에서 [[data-compression]] 개념과도 관련된다. Fail2Drive 벤치마크가 자율주행의 일반화 실패를 평가했다면, LEO는 인식 단계에서의 견고성 향상에 초점을 맞춘다.

## 🔗 관련 논문

- AdaRadar: Rate Adaptive Spectral Compression for Radar-based
- Fail2Drive: Benchmarking Closed-Loop Driving Generalization
- VectorWorld: Efficient Streaming World Model via Diffusion F
- Rectify, Don't Regret: Avoiding Pitfalls of Differentiable S

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/autonomous-driving.md|autonomous-driving]]
- [[concepts/autonomous-driving-perception.md|autonomous-driving-perception]]
- [[concepts/radar-perception.md|radar-perception]]
- [[concepts/multimodal-learning.md|multimodal-learning]]
- [[concepts/trajectory-prediction.md|trajectory-prediction]]
- [[concepts/data-compression.md|data-compression]]

---
_LLM 분석으로 재생성됨_
