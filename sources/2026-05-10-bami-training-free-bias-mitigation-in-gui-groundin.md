# BAMI: Training-Free Bias Mitigation in GUI Grounding

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06664v1

## 💡 핵심 인사이트

GUI 기밍의 실패는 단일한 능력 부족이 아니라 해상도 과잉에 의한 정밀도 편향과 인터페이스 복잡도에 의한 모호성 편향이라는 두 가지 구조적으로 독립된 편향으로 분해되며, MPD 귀인을 통해 편향 유형을 식별하면 훈련 없이 완화가 가능하다.

## 📖 분석

## BAMI: Training-Free Bias Mitigation in GUI Grounding

GUI 기밍 에이전트의 핵심 능력인 클릭·드래그 등의 좌표 예측에서, 기존 모델이 복잡한 GUI 환경(ScreenSpot-Pro 벤치마크)에서 보이는 성능 저하의 근원을 **Masked Prediction Distribution (MPD)** 귀인 방법으로 해부한 논문이다. 핵심 발견은 실패 모드가 단일한 능력 부족이 아니라 **두 가지 구조적으로 독립된 편향**—해상도 과잉에 의한 **정밀도 편향(precision bias)**과 복잡한 인터페이스 요소에 의한 **모호성 편향(ambiguity bias)**—으로 분해된다는 점이다.

이 분해는 [[entities/computer-use-agent|computer-use-agent]]의 실패 진단에 중요한 기여를 한다. 기존 연구가 CFG 해석 능력이나 도구 스키마 오버헤드 등 **인지적·시스템적 차원**의 병목을 식별했다면, BAMI는 **시각-공간적 입력 차원**에서 발생하는 편향을 정밀도-모호성 이분법으로 구조화한다. 특히 정밀도 편향은 [[entities/algorithm-system-translation-gap|algorithm-system-translation-gap]]의 변형으로 이해할 수 있다—모델의 기저 능력(저해상도에서 정상 동작)과 시스템 컨텍스트(고해상도 디스플레이) 간 번역에서 해상도라는 변수가 편향을 유발하는 구조적 간극이다.

훈련 없는(training-free) 완화라는 점에서 [[entities/on-device-inference|on-device-inference]] 및 기존 training-free 접근법들과 방법론적 계보를 공유하며, 귀인 기반 진단→편향 유형 식별→완화라는 파이프라인은 [[entities/mechanistic-interpretability|mechanistic-interpretability]]를 모델 내부가 아닌 입력-출력 분포 수준으로 확장하는 실용적 사례가 된다.

## 🔗 관련 논문

- 2026 04 23 chat2workflow a benchmark for generating executabl
- 2026 04 24 diagnosing cfg interpretation in llms
- 2026 04 24 swe chat coding agent interactions from real users
- 2026 04 23 safetyalfred evaluating safety conscious planning of multim

## 🏷️ 엔티티

- [[entities/gui-grounding.md|gui-grounding]]
- [[entities/masked-prediction-distribution.md|masked-prediction-distribution]]
- [[entities/precision-bias.md|precision-bias]]
- [[entities/ambiguity-bias.md|ambiguity-bias]]
- [[entities/bami.md|bami]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]

## 📐 개념

- [[concepts/training-free-bias-mitigation.md|training-free-bias-mitigation]]
- [[concepts/precision-bias.md|precision-bias]]
- [[concepts/ambiguity-bias.md|ambiguity-bias]]
- [[concepts/resolution-precision-tradeoff.md|resolution-precision-tradeoff]]
- [[concepts/interface-complexity-ambiguity.md|interface-complexity-ambiguity]]
- [[concepts/input-attribution-based-diagnosis.md|input-attribution-based-diagnosis]]

---
_LLM 분석으로 생성됨_
