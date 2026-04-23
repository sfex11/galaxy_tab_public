# AdaptToken: Entropy-based Adaptive Token Selection for MLLM Long Video Understanding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-31
**링크**: http://arxiv.org/abs/2603.28696v1

## 💡 핵심 인사이트

MLLM의 자기 불확실성(엔트로피)을 글로벌 토큰 선택과 적응적 조기 종료의 제어 신호로 활용함으로써, 학습 없이도 장기 비디오 이해의 효율성과 성능을 동시에 달성할 수 있다.

## 📖 분석

## AdaptToken: 엔트로피 기반 적응적 토큰 선택을 통한 MLLM 장기 비디오 이해

AdaptToken은 멀티모달 대형 언어 모델(MLLM)의 장기 비디오 이해를 위한 학습 불필요(training-free) 프레임워크다. 기존 방법들이 짧은 클립 내에서 프레임/토큰을 점수화하여 선택하는 방식이었다면, AdaptToken은 MLLM 자체의 **자기 불확실성(self-uncertainty)**을 전역 제어 신호로 활용하는 근본적으로 다른 접근을 취한다.

핵심 메커니즘은 두 가지다: (i) 멀리 떨어진 비디오 클립 간의 관련성을 비교할 수 있는 **엔트로피 기반 글로벌 토큰 선택**, (ii) 충분한 증거가 수집되면 처리를 중단하는 **적응적 조기 종료(early stopping)**. 이는 기존의 고정된 토큰 예산 방식과 달리, 질문의 난이도와 비디오 내용에 따라 계산량을 동적으로 조절한다.

이 연구는 비디오 VLM 효율화 연구의 새로운 방향을 제시한다. 기존 토큰 프루닝 연구([[concepts/token-pruning.md|token pruning]])가 공간-시간적 중요도 점수에 기반했다면, AdaptToken은 모델의 내부 불확실성이라는 정보 이론적 기준을 도입한다. 또한 불확실성 정량화([[concepts/uncertainty-quantification.md|uncertainty quantification]]) 개념을 추론 시 효율성 제어에 직접 연결한 점이 주목할 만하다. 학습 없이 작동한다는 점에서 기존 MLLM에 플러그인 형태로 적용 가능하며, 이는 장기 비디오 처리의 실용적 장벽을 크게 낮춘다.

## 🔗 관련 논문

- 2026 03 19 unified spatio temporal token scoring for efficien
- 2026 03 24 semantic token clustering for efficient uncertaint
- 2026 03 24 videoseek long horizon video agent with tool guide

## 🏷️ 엔티티

- [[entities/mllm.md|mllm]]

## 📐 개념

- [[concepts/token-pruning.md|token-pruning]]
- [[concepts/uncertainty-quantification.md|uncertainty-quantification]]
- [[concepts/video-vlm.md|video-vlm]]
- [[concepts/long-context.md|long-context]]
- [[concepts/video-understanding.md|video-understanding]]
- [[concepts/speculative-decoding.md|speculative-decoding]]

---
_LLM 분석으로 재생성됨_
