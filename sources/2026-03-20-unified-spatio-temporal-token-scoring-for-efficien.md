# Unified Spatio-Temporal Token Scoring for Efficient Video VLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-20
**링크**: http://arxiv.org/abs/2603.18004v1

## 💡 핵심 인사이트

ViT와 LLM을 관통하는 통합 시공간 토큰 스코어링으로, 비디오 VLM에서 시간적·공간적 중복 토큰을 동시에 제거하여 효율성과 성능을 양립시킨다.

## 📖 분석

## Unified Spatio-Temporal Token Scoring for Efficient Video VLMs

본 논문은 비디오 기반 비전-언어 모델(VLM)의 연산 효율성을 높이기 위한 통합 시공간 토큰 프루닝(token pruning) 프레임워크를 제안한다. 기존 토큰 프루닝 접근법은 크게 두 가지로 나뉘었다: (1) Vision Transformer(ViT) 내부에서만 프루닝을 수행하되 하류 비전-언어 태스크에 적응하지 못하는 방식, (2) LLM 내부에서만 프루닝하면서 ViT 출력은 그대로 유지하는 방식. 두 접근 모두 비디오의 시간적 중복성(temporal redundancy)을 종합적으로 처리하지 못하는 한계가 있었다.

본 연구는 ViT와 LLM을 관통하는 통합 스코어링 메커니즘을 도입하여, 공간적·시간적 차원 모두에서 토큰의 중요도를 평가하고 불필요한 토큰을 제거한다. 이를 통해 비디오 VLM의 계산 비용을 크게 줄이면서도 성능 저하를 최소화한다.

### 기존 Wiki와의 연결

이 연구는 [[Transformer]] 아키텍처의 효율성 개선과 직결된다. ViT와 LLM 모두 Transformer 기반이므로, 토큰 프루닝은 Transformer의 근본적 연산 병목을 해결하는 핵심 기법이다. 또한 비디오 이해 태스크에서의 효율적 추론은 LLM Agent가 멀티모달 입력을 실시간으로 처리해야 하는 시나리오와도 관련이 깊다. 최근 연구된 멀티모달 임베딩(MMEmb-R1) 및 시각 표현 학습(Steerable Visual Representations)과 상보적인 관계에 있으며, 특히 TriAttention의 효율적 추론 접근법과 방법론적 유사성을 공유한다.

## 🔗 관련 논문

- 2026 04 08 triattention efficient long reasoning with trigono
- 2026 04 09 mmemb r1 reasoning enhanced multimodal embedding w

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/video-understanding.md|video-understanding]]

---
_LLM 분석으로 재생성됨_
