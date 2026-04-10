# AdaRadar: Rate Adaptive Spectral Compression for Radar-based Perception

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17979v1

## 💡 핵심 인사이트

레이더 기반 자율주행 인지에서 가용 대역폭에 따라 압축률을 동적으로 조절하는 적응형 스펙트럼 압축 코덱을 제안하여, 저대역폭 환경에서도 고차원 레이더 데이터의 인지 성능을 보존한다.

## 📖 분석

## AdaRadar: Rate Adaptive Spectral Compression for Radar-based Perception

자율주행 시스템에서 레이더는 전천후 작동 특성과 거리·도플러 속도 측정 능력 덕분에 핵심 인지 모달리티로 자리잡고 있다. 그러나 고차원 원시 레이더 데이터의 방대한 양은 NPU 등 컴퓨팅 엔진으로의 통신 링크를 포화시키는 문제를 야기한다. 특히 저대역폭 인터페이스에서는 저해상도 Range-Doppler 프레임 몇 개만 전송 가능하도록 데이터 레이트가 설정되어 있어, 고차원 레이더 데이터를 효과적으로 활용하기 위한 범용 코덱이 부재한 상황이다.

AdaRadar는 이 문제를 해결하기 위해 **적응형 스펙트럼 압축(rate adaptive spectral compression)** 기법을 제안한다. 핵심 아이디어는 레이더 데이터의 스펙트럼 특성을 활용하여, 가용 대역폭에 따라 압축률을 동적으로 조절하면서도 인지 성능을 최대한 보존하는 것이다. 이는 단순한 데이터 압축을 넘어, 인지 태스크의 품질을 고려한 **인지 지향적 압축(perception-aware compression)** 패러다임에 해당한다.

이 연구는 자율주행의 센서 데이터 파이프라인 효율화라는 실용적 문제를 다루며, 레이더 데이터 처리에 딥러닝 기반 압축 기법을 적용한다는 점에서 신호 처리와 머신러닝의 교차점에 위치한다. 기존 Wiki의 [[sources/2026-04-10-cadence-context-adaptive-depth-estimation-for-navi.md|CADENCE]] 연구가 내비게이션을 위한 적응형 깊이 추정을 다뤘다면, AdaRadar는 레이더 모달리티에서의 적응형 데이터 압축이라는 상보적 접근을 제시한다. 두 연구 모두 '컨텍스트/상황에 따른 적응(adaptive)'이라는 공통 설계 철학을 공유한다.

## 🔗 관련 논문

- 2026 04 10 cadence context adaptive depth estimation for navi

## 📐 개념

- [[concepts/autonomous-driving-perception.md|autonomous-driving-perception]]
- [[concepts/data-compression.md|data-compression]]

---
_LLM 분석으로 재생성됨_
