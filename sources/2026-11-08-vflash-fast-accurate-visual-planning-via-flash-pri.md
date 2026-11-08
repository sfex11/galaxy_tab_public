# VFlash: Fast, Accurate Visual Planning via Flash Primitive Decoding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08449v1

## 💡 핵심 인사이트

프리미티브의 알려진 출력 구조 지식을 디코딩에 주입하면 좌표별 토큰 생성의 비용과 표현 손실을 동시에 제거할 수 있어, 시각 계획에서 속도와 정확성은 트레이드오프가 아니다.

## 📖 분석

# VFlash: Fast, Accurate Visual Planning via Flash Primitive Decoding

물리 AI(로봇 조작·자율주행)는 언어 대신 시각 계획 — 점, 바운딩 박스, 궤적 — 로 공간 목표를 표현하고 운동을 예측할 수 있다. 그러나 자회귀 VLM은 이를 좌표 토큰 단위로 생성하므로, 예측이 풍부해질수록 비용이 증가하는 구조적 병목([[autoregressive-paradigm-confinement]])이 발생한다.

VFlash는 Flash Primitive Decoding으로 프리미티브의 알려진 구조를 디코딩 시점에 활용하여 이 병목을 우회한다. 이는 접지 경로의 양극화를 완성한다 — VideoLVR([[latent-visual-reasoning]])이 입력 측에서 시각 증거의 잠재 표현 주입으로 텍스트 번역 손실을 회피했다면, VFlash는 출력 측에서 좌표의 자연어 토큰화 비용과 손실을 [[textual-coordinate-grounding]] 대비 프리미티브 단위 직접 생성으로 동시에 제거한다. 입출력 양단에서 접지가 텍스트 번역을 전제하지 않을 수 있음이 확정된다.

또한 [[primitive-level-generation]]과 [[structure-informed-decoding]]의 원천 정의를 확립하며, 연속 공간을 이산 토큰으로 번역하는 [[action-tokenization]]·[[representation-contract]] 계열의 비용 문제에 구조 지식 기반 해법을 제시한다. 물리 도메인에서 [[thinking-acting-gap]]을 좁히고 [[visual-planning]]의 효율 지평([[video-inference-efficiency]], [[token-efficiency]])을 확장하는 실용적 경로다.

## 🔗 관련 논문

- VideoLVR: Latent Visual Reasoning over Grounded Video Evidence

## 🏷️ 엔티티

- [[entities/vflash.md|vflash]]
- [[entities/visual-grounding.md|visual-grounding]]

## 📐 개념

- [[concepts/visual-planning.md|visual-planning]]
- [[concepts/primitive-level-generation.md|primitive-level-generation]]
- [[concepts/structure-informed-decoding.md|structure-informed-decoding]]
- [[concepts/textual-coordinate-grounding.md|textual-coordinate-grounding]]
- [[concepts/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[concepts/autoregressive-paradigm-confinement.md|autoregressive-paradigm-confinement]]
- [[concepts/action-tokenization.md|action-tokenization]]
- [[concepts/representation-contract.md|representation-contract]]
- [[concepts/parallel-decoding.md|parallel-decoding]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/video-inference-efficiency.md|video-inference-efficiency]]

---
_LLM 분석으로 생성됨_
