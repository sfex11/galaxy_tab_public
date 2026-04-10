# Unified Spatio-Temporal Token Scoring for Efficient Video VLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.18004v1

## 💡 핵심 인사이트

ViT와 LLM을 분리하지 않고 통합된 시공간 토큰 스코어링으로 비디오 VLM의 계산 효율성을 달성한 점이 핵심이며, 이는 기존 단일 단계 프루닝의 정보 손실 문제를 해결한다.

## 📖 분석

## Unified Spatio-Temporal Token Scoring for Efficient Video VLMs

본 논문은 비디오 기반 비전-언어 모델(VLM)에서 토큰 프루닝(token pruning)을 통한 계산 효율성 향상을 다룬다. 기존 접근법들은 토큰 프루닝을 (1) Vision Transformer(ViT) 내부에서만 수행하거나 (2) LLM 내부에서만 수행하는 이분법적 한계를 가졌다. 본 연구는 ViT와 LLM을 아우르는 **통합 시공간 토큰 스코어링(Unified Spatio-Temporal Token Scoring)** 프레임워크를 제안하여, 비디오의 시간적 중복성(temporal redundancy)을 효과적으로 제거한다.

### 핵심 기여

- **통합 프루닝 전략**: ViT 단계와 LLM 단계를 분리하지 않고, 시공간 차원에서 일관된 토큰 중요도 스코어링을 수행한다. 이를 통해 비전 인코더 출력과 언어 모델 입력 간의 정보 손실을 최소화한다.
- **시간적 중복성 활용**: 비디오 프레임 간 반복되는 시각 정보를 식별하고 제거함으로써, 긴 비디오에서도 효율적인 추론이 가능하다.
- **비전-언어 태스크 적응**: 기존 ViT 전용 프루닝이 행동 인식 등 단일 모달 태스크에 한정된 반면, 본 방법은 비디오 QA, 비디오 캡셔닝 등 멀티모달 태스크에 직접 최적화된다.

### 기존 Wiki와의 관계

[[Transformer]] 아키텍처의 효율성 문제를 비디오 VLM 맥락에서 다루며, ViT와 LLM 양쪽 모두의 토큰 처리를 통합한다는 점에서 Transformer 연구의 확장이다. 또한 2026-04-08의 **TriAttention** 논문이 긴 추론(long reasoning)에서 삼각함수 기반 효율적 어텐션을 다뤘다면, 본 논문은 긴 비디오 입력에서의 토큰 효율성이라는 상보적 문제를 해결한다.

## 🔗 관련 논문

- 2026 04 08 triattention efficient long reasoning with trigono

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/video-vlm.md|video-vlm]]

---
_LLM 분석으로 재생성됨_
