# Legibility is Not Interpretability: Comparing Judged and Actual Importance in Chain-Of-Thought Reasoning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04194v1

## 💡 핵심 인사이트

CoT 추론 흔적의 가독성은 해석가능성이 아니며, LLM judge가 판단한 스텝 중요도는 실제 인과적 기여와 발산하므로 judge·PRM·critic 전반이 공유하는 '텍스트가 기능을 담는다'는 근본 전제가 무너진다.

## 📖 분석

# Legibility is Not Interpretability: Comparing Judged and Actual Importance in Chain-Of-Thought Reasoning (2026-09-06)

## 핵심 주장

CoT 추론 흔적은 모델의 사고 과정에 대한 '가독 가능한 창'처럼 보이며, LLM judge 기반 오류 진단·충실도 평가·프로세스 보상 모델(PRM)·생성적 비평가가 이를 그대로 활용한다. 본 논문은 이 관행의 근본 전제 — "추론 스텝의 텍스트가 그 기능적 역할에 대한 정보를 인코딩한다" — 를 검증한다. LLM judge가 판단한 스텝 중요도(judged importance)와 개입 기반으로 측정한 실제 중요도(actual importance)를 비교하여 두 값이 구조적으로 발산함을 보인다. 즉 **가독성(legibility)은 해석가능성(interpretability)이 아니다**.

## 기존 Wiki와의 관계

- [[llm-as-judge]]: 추이성 위반이 '측정 일관성'의 문제였다면, 본 논문은 측정 대상 자체가 텍스트에 실체화되지 않는 '측정 가능성' 문제로 격상시킨다.
- [[process-reward-model]]: 단계별 감독이 실제 기능적 기여가 아닌 판독 가능한 서사에 최적화될 위험을 제시한다.
- [[reasoning-integrity]]: 프로세스 제어·논리 부분공간 논의에 '표면 정합성 ≠ 인과 무결성' 구분을 추가한다.
- [[meaning-insensitive-metric]]: WER의 '의미 무감각성'과 동형인 '기능 무감각성'의 추론 평가판이다.
- [[evaluator-assumption]]: '텍스트가 기능을 담는다'는 평가자의 암묵적 가정을 실증적으로 해체한다.

## 구조적 연결

"Cited but Not Verified"(인용 구조의 표면 완비성 vs 실제 검증)와 동일한 '표면 완비성 오인' 패턴의 추론 도메인 발현이다. judge·PRM·critic이 공유하는 전제가 깨진 사례로, step-level 감독 설계에는 개입 기반 검증의 병행이 요구된다.

## 🔗 관련 논문

- When LLMs Stop Following Steps: A Diagnostic Study of Procedural Execu
- Cited but Not Verified: Parsing and Evaluating Source Attrib
- Evaluation of Automatic Speech Recognition Using Generative
- Cliff: Learning Process Rewards from the First Mistake
- Discovering a Shared Logical Subspace: Steering LLM Logical

## 🏷️ 엔티티

- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/reasoning-integrity.md|reasoning-integrity]]
- [[entities/process-reward-model.md|process-reward-model]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/judged-actual-importance-divergence.md|judged-actual-importance-divergence]]
- [[concepts/step-importance-causal-verification.md|step-importance-causal-verification]]
- [[concepts/surface-completeness-misreading.md|surface-completeness-misreading]]

---
_LLM 분석으로 생성됨_
