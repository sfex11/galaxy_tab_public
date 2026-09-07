# A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Miniature Ackermann Vehicle

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04147v1

## 💡 핵심 인사이트

End-to-end 자율주행 연구의 실질 병목은 알고리즘이 아니라 실험 인프라의 비용·접근성이며, 미니어처 물리 차량과 디지털 트윈의 쌍 구성으로 sim-to-real 검증 루프를 개인 연구자 수준까지 민주화할 수 있다.

## 📖 분석

본 논문은 미니어처 Ackermann 차량 기반 저비용·개방형 end-to-end 자율주행 실험 플랫폼을 제시한다. 물리 차량, 인쇄 도시 트랙, 데이터 수집 도구, 궤적 등록, Webots 디지털 트윈을 결합해 시뮬레이션 기반 방법론과 실차 실행을 연결하는 통제된 실험 환경을 구축하고, command-conditioned behavior cloning을 기준선으로 제공한다.

Wiki 관점에서 세 축으로 기존 논의를 확장한다. 첫째, [[autonomous-driving]] 논의가 LiDAR 인지-배포 간극에 집중해 왔다면, 본 논문은 '연구 인프라 민주화'라는 새 차원을 추가한다. 둘째, [[end-to-end-vla-training]] 계열이 자율주행을 연속적·물리제약 도메인으로 확장했던 것에 실증 검증 무대를 제공한다. 셋째, [[closed-loop-evaluation]]에 시뮬레이션 사전 검증-실차 실행의 이중 루프라는 물리적 실현 경로를 제시한다.

핵심은 [[miniaturization-accessibility]]다: end-to-end 자율주행 연구의 실질 병목이 알고리즘이 아닌 실험 인프라의 비용·접근성에 있으며, 미니어처 플랫폼과 디지털 트윈의 쌍 구성이 [[sim-to-real-validation-infrastructure]]를 개인 연구자 수준으로 하향 평준화함을 보여준다. 이는 [[physical-digital-twin-pairing]]의 대표적 구현 사례가 된다.

## 🔗 관련 논문

- Toward Robust LiDAR Semantic Segmentation for Real-World Deployment: E
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- Corner Cases: Headland Coverage Path Planning for Autonomous

## 🏷️ 엔티티

- [[entities/miniature-vehicle-research-platform.md|miniature-vehicle-research-platform]]
- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]

## 📐 개념

- [[concepts/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]
- [[concepts/physical-digital-twin-pairing.md|physical-digital-twin-pairing]]
- [[concepts/miniaturization-accessibility.md|miniaturization-accessibility]]
- [[concepts/command-conditioned-behavior-cloning.md|command-conditioned-behavior-cloning]]
- [[concepts/open-experimental-platform.md|open-experimental-platform]]

---
_LLM 분석으로 생성됨_
