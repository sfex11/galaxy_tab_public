# VectorWorld: Efficient Streaming World Model via Diffusion Flow on Vector Graphs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17652v1

## 💡 핵심 인사이트

벡터 그래프 기반 확산 플로우를 통해 실시간 예산 내에서 동작하는 스트리밍 월드 모델을 구현하여, 자율주행 폐루프 시뮬레이션의 세 가지 핵심 병목(초기화 불일치, 샘플링 지연, 운동학적 오류 누적)을 동시에 해결했다.

## 📖 분석

## VectorWorld: Efficient Streaming World Model via Diffusion Flow on Vector Graphs

자율주행 정책의 폐루프(closed-loop) 평가는 단순 로그 리플레이를 넘어선 인터랙티브 시뮬레이션을 요구한다. 기존 생성형 월드 모델들은 폐루프 환경에서 (i) 히스토리 없는 초기화로 인한 정책 입력 불일치, (ii) 다단계 샘플링 지연으로 실시간 예산 초과, (iii) 장기 호라이즌에서의 운동학적 비현실성 누적 등의 문제로 성능이 저하된다.

VectorWorld는 이러한 한계를 극복하기 위해 **벡터 그래프 기반 확산 플로우(diffusion flow)** 를 활용한 스트리밍 월드 모델을 제안한다. 핵심 아이디어는 자차 중심 64m×64m 영역을 벡터 그래프로 표현하고, 이를 점진적(incremental)으로 생성하는 것이다. 래스터 이미지 대신 벡터 표현을 채택함으로써 구조적 일관성과 계산 효율성을 동시에 확보한다.

이 연구는 **시뮬레이션 기반 자율주행 평가**의 실용성을 크게 높인다는 점에서 의의가 있다. 실시간 예산 내에서 동작하는 월드 모델은 강화학습 기반 정책 훈련과 평가 모두에 핵심 인프라가 된다. 특히 확산 모델의 추론 지연 문제를 스트리밍 방식으로 해결한 접근은, 생성 모델의 실시간 응용이라는 더 넓은 연구 흐름과 맞닿아 있다.

벡터 그래프 표현은 기존 포인트 클라우드나 래스터 맵 대비 장면의 토폴로지 정보를 명시적으로 보존하며, 이는 장기 시뮬레이션에서의 누적 오류를 줄이는 데 기여한다.

## 🔗 관련 논문

- 2026 04 10 robust quadruped locomotion via evolutionary reinf
- 2026 04 10 cadence context adaptive depth estimation for navi

## 📐 개념

- [[concepts/world-model.md|world-model]]
- [[concepts/diffusion-model.md|diffusion-model]]

---
_LLM 분석으로 재생성됨_
