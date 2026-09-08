# Necessary or Sufficient? Evaluating LLM Explanations With Behavioural Evidence

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05385v1

## 💡 핵심 인사이트

설명에 명명된 요인의 필요성(변경 시 출력 변경)과 충분성(요인 자체가 출력 재현)은 분리된 인과적 속성이며, 텍스트 판독이 아닌 행동 증거 기반 개입 검증으로만 설명의 실제 행동 일치성을 판정할 수 있다.

## 📖 분석

## Necessary or Sufficient? Evaluating LLM Explanations With Behavioural Evidence (2026-09-08)

에이전트 워크플로우 내 LLM 의사결정 구성요소가 산출하는 설명의 명명된 요인(named factors)이 실제 의사결정 행동과 일치하는지를 **필요성**과 **충분성**이라는 두 인과적 기준으로 분해해 검증한다.

### 핵심 구분
- **필요성**: 해당 요인을 변경하면 출력이 바뀌는가 (necessity)
- **충분성**: 해당 요인 자체만으로 출력을 재현할 수 있는가 (sufficiency)

두 속성은 독립적이며, 설명 텍스트의 표면 판독만으로는 구별 불가능하다. 행동 증거(반사실적 개입)를 통한 검증으로만 분리 판정 가능하다.

### Wiki와의 관계
[[legibility-interpretability-gap]] 논문(2026-09-07)이 judge가 판단한 단계 중요도와 개입 실험으로 측정한 실제 중요도의 발산을 실증했다면, 본 논문은 설명 평가를 '일치/불일치' 이분법에서 필요성·충분성의 인과 지위 공간으로 정밀화한다. [[step-importance-causal-verification]]의 방법론적 후속으로, 개입 검증의 대상을 reasoning step 중요도에서 설명에 명명된 요인의 지위로 확장한다. 이는 [[cot-as-translated-report]] 인식론 — 가독적 텍스트가 계산의 실재를 전달한다는 보장 부재 — 을 에이전트 운영 계층으로 확장하는 실증 사례다.

### 실무적 함의
운영자가 설명을 모니터링·오류 진단·에스컬레이션 결정에 사용하는 [[human-oversight]] 인프라에서, 설명-행동 불일치는 감독의 실효성을 은밀하게 훼손한다. [[process-reward-model]]과 [[judged-actual-importance-divergence]]가 지적한 감독 신호 취약성을 설명 평가 도메인에서 반복 확인시킨다.

## 🔗 관련 논문

- Legibility is Not Interpretability: Comparing Judged and Actual Import
- Judge Instrument Reliability
- Preregistered Measurement
- Clean Engineering, Unstable Measurement

## 🏷️ 엔티티

- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/step-importance-causal-verification.md|step-importance-causal-verification]]
- [[entities/judged-actual-importance-divergence.md|judged-actual-importance-divergence]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/human-oversight.md|human-oversight]]
- [[entities/process-reward-model.md|process-reward-model]]
- [[entities/necessity-sufficiency-decoupling.md|necessity-sufficiency-decoupling]]

## 📐 개념

- [[concepts/necessity-sufficiency-decoupling.md|necessity-sufficiency-decoupling]]
- [[concepts/behavioural-explanation-verification.md|behavioural-explanation-verification]]
- [[concepts/counterfactual-factor-testing.md|counterfactual-factor-testing]]

---
_LLM 분석으로 생성됨_
