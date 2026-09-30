# TokenCast: Forecasting Token Consumption During LLM Agent Execution

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35760v1

## 💡 핵심 인사이트

토큰 소비는 단일 호출의 속성이 아니라 행동 선택×컨텍스트 성장의 곱셈으로 창발하는 궤적 수준 속성이므로, 비용 예측은 합성 가능한 모델과 실행 중 지속 수정이라는 런타임 갱신 구조를 필수로 요구한다.

## 📖 분석

동일 태스크에서 토큰 소비가 10배 이상 변동한다는 실측은 '같은 요청은 같은 비용'이라는 [[request-centric-optimization]]의 전제가 에이전트 워크로드에서 붕괴함을 보여준다. 비용은 단일 호출의 속성이 아니라, 도구 피드백에 따라 선택되는 다음 행동(행동 축)과 성장하는 컨텍스트가 후속 호출마다 입력 크기를 팽창시키는 구조(인프라 축)가 곱셈으로 결합된 궤적 수준 창발 속성이다 — [[behavior-infrastructure-dual-cost-model]]의 이중 구조를 예측 가능한 형태로 형식화한 사례다. TokenCast의 핵심은 두 가지다. (1) 비용 모델을 합성 가능한(composable) 형태로 학습하되, 사전 예측에 고정하지 않고 실행 중 관측으로 지속 수정하는 런타임 갱신 구조 — '예측' 자체가 [[adaptive-inference]]의 대상이 됨. (2) 비용 예측이 서빙의 계획 입력이 되면, Pythia의 의미적 예측([[predictability-driven-serving]])에 이어 '얼마나 소비할 것인가'라는 제2 예측 축이 열려 [[agent-native-serving]]의 설계 공간이 확장된다. [[retry-context-accumulation-loop]]의 폭주 위험을 사후 정산이 아닌 중도 감지로 관리 가능하게 하며, [[inference-budget-progressive-investment]]의 예산 투입 판단에 정량적 근거를 제공한다.

## 🔗 관련 논문

- Pythia: Toward Predictability-Driven Agent-Native LLM Serving
- EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction
- Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo

## 🏷️ 엔티티

- [[entities/token-consumption-forecasting.md|token-consumption-forecasting]]
- [[entities/behavior-infrastructure-dual-cost-model.md|behavior-infrastructure-dual-cost-model]]
- [[entities/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[entities/predictability-driven-serving.md|predictability-driven-serving]]
- [[entities/agent-native-serving.md|agent-native-serving]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[entities/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]

## 📐 개념

- [[concepts/token-consumption-forecasting.md|token-consumption-forecasting]]
- [[concepts/behavior-infrastructure-dual-cost-model.md|behavior-infrastructure-dual-cost-model]]
- [[concepts/predictability-driven-serving.md|predictability-driven-serving]]
- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/retry-context-accumulation-loop.md|retry-context-accumulation-loop]]
- [[concepts/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]
- [[concepts/request-centric-optimization.md|request-centric-optimization]]
- [[concepts/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[concepts/complexity-meta-cognition.md|complexity-meta-cognition]]

---
_LLM 분석으로 생성됨_
