# Beyond One-Size-Fits-All: Sample-Adaptive Strategy Routing for Vision Token Pruning in MLLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10346v1

## 💡 핵심 인사이트

평균 정확도 최고의 프루닝 전략이 모든 샘플에서 최선이 아니라는 샘플별 상보성의 발견이, 프루닝의 최적화 단위를 토큰 수준에서 전략 라우팅 수준으로 격상시킨다.

## 📖 분석

## 샘플 적응적 전략 라우팅: 프루닝의 메타-계층 도입

MLLM 비전 토큰 프루닝 연구에 두 축의 기여를 한다.

**적응 추론의 전략 계층.** 기존 [[adaptive-inference]] 논의는 외부 환경 반응(CADENCE)과 내부 압축 상태 반응(SpecKV)으로 확장되어 왔다. 본 논문은 적응 대상을 파라미터 수준에서 **전략 선택 수준**으로 격상시킨다 — 입력 샘플 특성을 관찰해 어떤 프루닝 전략을 적용할지 라우팅하는 것은 [[algorithm-level-adaptation]]의 구체적 실현이며, [[computation-unit-meta-selection]]의 메타-선택 대상을 '무엇을 실행할까'에서 '무엇을 제거할까'로 확장한다. [[adaptive-control-hierarchy]] 관점에서 이는 단일 방법 계열 내부의 중간 제어 계층이다.

**평균 지표의 은폐성 실증.** 평균 벤치마크 정확도로 프루닝 기법을 순위 매기는 관행이 **샘플별 상보성**을 은폐함을 보인다 — 평균 최고 전략조차 일부 샘플에서는 열위다. 이는 [[cross-domain-ranking-fallacy]]가 진단한 '집계 순위가 이질성을 소각'하는 구조를 도메인 간에서 샘플 간으로 미시화하며, [[statistical-ranking-indistinguishability]]에 방법론 비교 차원의 근거를 추가한다.

[[token-pruning]]의 설계 질문을 '어떤 토큰을 제거할까'에서 '어떤 전략으로 제거할까'로 상위 계층으로 이동시킨다.

## 🔗 관련 논문

- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Selection
- CADENCE: Context-Adaptive Depth Estimation for Navigation and Mapping
- Make Your LVLM KV Cache More Lightweight
- Why Global LLM Leaderboards Are Misleading: Small Portfolios
- Select to Think: Unlocking SLM Potential with Local Sufficiency
- ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding

## 🏷️ 엔티티

- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/algorithm-level-adaptation.md|algorithm-level-adaptation]]
- [[entities/token-pruning.md|token-pruning]]
- [[entities/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[entities/cross-domain-ranking-fallacy.md|cross-domain-ranking-fallacy]]
- [[entities/statistical-ranking-indistinguishability.md|statistical-ranking-indistinguishability]]

## 📐 개념

- [[concepts/sample-wise-complementarity.md|sample-wise-complementarity]]
- [[concepts/strategy-routing.md|strategy-routing]]
- [[concepts/average-metric-concealment.md|average-metric-concealment]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-11-why-is-video-still-so-expensive-a-survey-of-infere]]: 비디오 LLM 효율화 서베이가 토큰 프루닝·적응적 추론을 핵심 메커니즘으로 제시하는 가운데, 본 논문은 이를 샘플 적응적 전략 라우팅이라는 메타 계층으로 구체화한 사례다.
