# Select to Think: Unlocking SLM Potential with Local Sufficiency

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26940v1

## 💡 핵심 인사이트

SLM의 추론 한계가 모델 용량의 부족이 아니라 자신의 분포 내에서 최적 토큰을 선택하지 못하는 문제라면, 분포 밖 확장(LLM 호출·증류)이 아닌 분포 내 최적화(local sufficiency)로도 추론 격차를 구조적으로 좁힐 수 있다.

## 📖 분석

# Select to Think: Local Sufficiency로 SLM 추론 잠금 해제

## 기존 Wiki와의 관계

이 논문은 SLM(소형 언어 모델)과 LLM 간의 추론 격차를 해소하기 위한 세 번째 경로를 제시한다. 기존 Wiki가 기술한 두 접근 — (1) 추론 발산점에서 LLM을 외부 호출하는 방식(speculative-decoding 계열)과 (2) 표준 지식 증류(knowledge-distillation) — 는 각각 지연·비용 문제와 SLM 용량 한계에 직면해 왔다. 본 논문은 이 둘 사이의 새로운 지점을 찾는다.

## 핵심 기여: Local Sufficiency

SLM 자신의 주변 분포 P(y) 내에서 추론에 '국소적으로 충분한' 토큰을 선택하는 방식으로, 외부 LLM 호출 없이도 추론 품질을 향상시킨다. 이는 [[entities/marginal-distribution-ceiling|주변 분포 성능 상한선]] 개념과 직접 연결된다 — SLM의 P(y) 천장을 높이는 것이 아니라, 기존 P(y) 내에서 더 잘 선택함으로써 천장에 더 가깝게 도달하는 전략이다.

## 다른 논문과의 연결점

- **Carbon-Taxed Transformers**: 압축 후 정확도 저하 문제에 대해 본 논문의 토큰 선택이 보완적 해법이 될 수 있다
- **Tool Attention**: 도구 스키마 선택의 지연 로딩과 본 논문의 토큰 선택이 동일한 철학 — '불필요한 것을 배제하고 충분한 것만 선택' — 을 공유한다
- **Exploration-Absorption Decoupling**: RL이 경로를 개척하고 사후학습이 흡수하는 패러다임에서, 본 논문은 SLM이 자신의 분포 내에서 '흡수 가능한' 토큰을 식별하는 메커니즘을 제공한다

## 의의

SLM 추론이 P(y|x)의 재매개변수화 문제가 아니라 P(y) 내 선택 문제로 재구성됨을 보여주며, [[entities/on-device-inference|온디바이스 추론]]의 실질적 성능 상한을 모델 크기 변경 없이 끌어올리는 구조적 경로를 제공한다.

## 🔗 관련 논문

- 2026-04-30-carbon-taxed-transformers-a-green-compression-pipe.md
- 2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md
- 2026-04-30-pythia-toward-predictability-driven-agent-native-l.md

## 🏷️ 엔티티

- [[entities/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/token-pruning.md|token-pruning]]
- [[entities/model-compression.md|model-compression]]
- [[entities/local-sufficiency.md|local-sufficiency]]

## 📐 개념

- [[concepts/local-sufficiency.md|local-sufficiency]]
- [[concepts/token-selection-reasoning.md|token-selection-reasoning]]
- [[concepts/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[concepts/distribution-internal-optimization.md|distribution-internal-optimization]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-05-01-turning-the-tide-cross-architecture-distillation-f]]: 두 논문 모두 거대 모델에 의존하지 않고 효율적인 모델(SLM 또는 경량화된 모델)을 구현하기 위해, 기존 표현 공간의 한계를 재정의하거나 분포 내 최적화를 통해 모델 간 격차를 줄이는 대안적 압축 및 최적화 경로를 제시한다.
