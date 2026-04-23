# Interval POMDP Shielding for Imperfect-Perception Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20728v1

## 💡 핵심 인사이트

유한 레이블 데이터에서 도출된 인지 확률의 신뢰 구간을 POMDP의 불확실성으로 직접 편입함으로써, 완전한 인지 모델 없이도 provably safe shielding이 가능하다는 것을 보이며, 이는 '인지 불확실성을 안전 보장의 구조적 변수로 흡수'하는 패러다임 전환이다.

## 📖 분석

# Interval POMDP Shielding for Imperfect-Perception Agents

## 정의
학습된 인지(perception) 모델의 오분류 가능성을 고려하여, 자율 시스템의 행동이 안전성을 위반할 가능성이 있으면 실시간으로 차단하는 shielding 프레임워크. 유한 레이블 데이터로부터 인지 결과의 확률에 대한 신뢰 구간(confidence interval)을 구축하고, 이를 Interval POMDP로 모델링하여 확률적 안전성을 보장한다.

## 기존 Wiki와의 관계

### MDP → POMDP로의 확장
기존 [[concepts/markov-decision-process.md|markov decision process]] 엔티티가 다루는 완전 관측 설정에서, 부분 관측(Partially Observable) 설정으로 확장한다. 동시에 2026-04-23의 "Planning in entropy-regularized MDP" 논문과 대비되는 점이 있다: 해당 논문이 엔트로피 정규화로 계획의 탐색성을 제어한다면, 본 논문은 인지 불확실성 자체를 구간으로 모델링하여 안전성을 형식적으로 보장한다.

### AI Safety: 사후 평가에서 사전 차단으로
[[concepts/ai-safety.md|ai safety]] 엔티티에서 SafetyALFRED(2026-04-23)가 LLM 계획의 사후 안전 평가 방법론의 한계를 노출했다면, 본 논문은 반대 방향—행동 실행 전에 확률적 보장 하에 차단하는 사전 shielding—을 제시한다. 이는 [[concepts/post-hoc-guardrail-limitation.md|post hoc guardrail limitation]] 개념의 구조적 대안으로 위치할 수 있다.

### Controlled Autonomy와의 연결
[[concepts/controlled-autonomy.md|controlled autonomy]] 패러다임 내에서 shielding은 무제약 자율성과 완전 분리 사이의 실용적 중간 지점을 제공한다: 에이전트의 계획 능력은 그대로 유지하되, 실행 시점에서 인지 불확실성에 기반한 안전 경계를 강제한다.

### Uncertainty Quantification의 실제 적용
[[concepts/uncertainty-quantification.md|uncertainty quantification]] 개념을 추상적 척도가 아닌 구체적인 안전 보장 메커니즘으로 변환한다. 유한 데이터에서의 신뢰 구간이 곧 안전 shield의 보수성(conservatism)을 결정하는 구조적 변수가 된다.

## 핵심 기여
완전한 인지 모델을 전제하는 기존 formal verification과, 인지 불확실성을 무시하는 기존 shielding 사이의 간극을 Interval POMDP로 메운다. 데이터가 유한하다는 현실적 제약을 안전 보장의 일부로 흡수하는 접근이 핵심이다.

## 🔗 관련 논문

- 2026-04-23-safetyalfred-evaluating-safety-conscious-planning-.md
- 2026-04-23-planning-in-entropy-regularized-markov-decision-pr.md
- 2026-04-07-minimal-information-control-invariance-via-vector-.md

## 🏷️ 엔티티

- [[entities/markov-decision-process.md|markov-decision-process]]
- [[entities/ai-safety.md|ai-safety]]
- [[entities/safety-critical-control.md|safety-critical-control]]
- [[entities/formal-verification.md|formal-verification]]
- [[entities/pomdp.md|pomdp]]
- [[entities/embodied-ai.md|embodied-ai]]

## 📐 개념

- [[concepts/interval-pomdp.md|interval-pomdp]]
- [[concepts/shielding.md|shielding]]
- [[concepts/perception-uncertainty.md|perception-uncertainty]]
- [[concepts/confidence-interval-safety.md|confidence-interval-safety]]
- [[concepts/imperfect-perception.md|imperfect-perception]]
- [[concepts/provably-safe-shielding.md|provably-safe-shielding]]

---
_LLM 분석으로 생성됨_
