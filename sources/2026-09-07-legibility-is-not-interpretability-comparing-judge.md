# Legibility is Not Interpretability: Comparing Judged and Actual Importance in Chain-Of-Thought Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04194v1

## 💡 핵심 인사이트

CoT trace의 가독성(legibility)은 해석가능성(interpretability)이 아니며, LLM judge가 판단한 단계 중요도와 인과적 개입으로 측정된 실제 기능적 중요도가 체계적으로 발산함으로써, 텍스트 기반 step-level 평가·보상·감독 체계 전반이 잘못된 프록시 위에 서 있음이 드러난다.

## 📖 분석

이 논문은 Chain-of-Thought 추론에서 '가독성(legibility)'과 '해석가능성(interpretability)'의 구조적 분리를 실증한다. LLM judge가 reasoning trace에서 중요하다고 판단하는 단계와, 인과적 개입으로 측정한 실제 기능적 중요도가 체계적으로 발산함을 보여준다. 이는 trace 텍스트가 계산의 기능적 역할 정보를 담고 있다는 Process Reward Model·LLM judges·generative critics의 공통 전제를 직접 공격한다.

Wiki 관점에서 이 논문의 위치는 명확하다. [[benchmark-specification-gap]]의 추론 평가 도메인 발현으로, 측정 프록시(텍스트 가독성)와 실제 목표(기능적 중요도)의 단절이 reasoning 단계 수준에서 입증된다. 동시에 [[surface-completeness-misreading]]의 직접적 구현 사례로, trace의 표면적 완결성이 기능적 중요도로 오독되는 메커니즘을 제공한다.

[[reasoning-integrity]] 계열(Box Maze 등)은 추론 과정의 무결성을 관찰 가능한 제약으로 강제하려 했으나, 본 논문은 그 관찰 계층 자체(trace 텍스트)가 기능 계층과 분리되어 있음을 노출한다. 이는 [[agent-execution-semantic-opacity]]의 LLM 내부 버전으로 해석 가능하다 — 실행 궤적의 불투명성이 모델 내부 추론 궤적에서도 동일하게 발생한다.

방법론적으로, 실제 중요도 판별에는 개입적(interventional) 검증이 필요함을 보여 [[causal-mechanistic-interpretability]]의 필요성을 강화하며, 해석가능성을 '판독 문제'에서 '개입 문제'로 재정의한다. 이는 [[judge-instrument-reliability]]의 측정기 신뢰성 논의를 '일관성' 차원에서 '측정 대상 타당성' 차원으로 확장한다.

## 🔗 관련 논문

- Clean Engineering, Unstable Measurement: A Preregistered Reliability Framework
- When LLMs Stop Following Steps: A Diagnostic Study of Procedural Execution
- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineer
- Cited but Not Verified: Parsing and Evaluating Source Attribution in LLM
- Cliff: Learning Process Rewards from the First Mistake

## 🏷️ 엔티티

- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/process-reward-model.md|process-reward-model]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/judged-actual-importance-divergence.md|judged-actual-importance-divergence]]
- [[entities/step-importance-causal-verification.md|step-importance-causal-verification]]
- [[entities/surface-completeness-misreading.md|surface-completeness-misreading]]
- [[entities/reasoning-integrity.md|reasoning-integrity]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]

## 📐 개념

- [[concepts/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[concepts/judged-actual-importance-divergence.md|judged-actual-importance-divergence]]
- [[concepts/step-importance-causal-verification.md|step-importance-causal-verification]]
- [[concepts/process-reward-model.md|process-reward-model]]
- [[concepts/reasoning-chain-evaluation.md|reasoning-chain-evaluation]]
- [[concepts/interpretability-verifiability-substitution.md|interpretability-verifiability-substitution]]

---
_LLM 분석으로 생성됨_
