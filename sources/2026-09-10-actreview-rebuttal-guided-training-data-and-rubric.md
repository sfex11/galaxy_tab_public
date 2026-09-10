# ActReview: Rebuttal-Guided Training Data and Rubric Rewards for Actionable Peer Review Generation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-10
**링크**: http://arxiv.org/abs/2609.09076v1

## 💡 핵심 인사이트

피어 리뷰의 rebuttal은 리뷰어의 암묵적 기준(어떤 진단이 유효하고 어떤 수정이 수용 가능한가)을 자연 감독 라벨로 외면화하며, 이를 post-training에 활용하면 LLM 피드백을 '약점 식별'에서 '수정 유도'로 격상시킬 수 있다.

## 📖 분석

# ActReview: Rebuttal-Guided Training Data and Rubric Rewards (2026-09-10)

LLM 사전심사(self-review) 맥락에서 피드백의 품질 기준을 '약점 식별'에서 '수정 유도(actionable)'로 격상시킨다. 과제를 진단 주장 생성(diagnostic claim generation)과 수정 제안 생성(revision suggestion generation)의 두 하위 태스크로 분해하여, 리뷰의 산출 단위가 판정이 아닌 진단-치유 쌍임을 명시한다.

## 핵심 메커니즘: Rebuttal의 감독 신호화

저자의 rebuttal은 리뷰어 진단에 대한 실제 대응 기록이므로, '어떤 진단이 유효하고 어떤 수정이 대응 가능한가'에 대한 자연적 감독 라벨이다. 이는 [[tacit-criteria-surfacing]]의 학습 데이터 버전 — 암묵적 리뷰 기준이 상호작용 흔적에서 형식화된다. [[human-trace-external-anchoring]] 관점에서 rebuttal은 자기 생성 데이터의 순환 타당성을 절단하는 인간 근거 닻으로 기능한다.

## Wiki 내 위치

- [[llm-as-judge]]의 확장: 판정형 출력(점수/수용 여부)에서 진단+수정의 이중 출력으로
- [[llm-as-code-reviewer]]와 평행 구조: SWE-Gate의 리뷰 제약 준수와 동형 — 수용 가능한 수정 제안이 리뷰의 실제 수용 단위
- [[rlvr]]·[[process-reward-model]]의 도메인 확장: rubric reward는 정답 부재 도메인에서의 검증 가능 보상이나, [[reward-hacking]] 표면(루브릭을 충족하는 표면적 피드백)을 수반
- [[scientific-workflow-agent]]: 연구 수명주기에 pre-submission 품질 게이트 계층 추가

진단과 수정의 분리는 [[evaluation-deployment-unit-mismatch]]를 조작 가능한 형태로 전환한다 — 리뷰 품질의 측정 축(진단 정확성 vs 수정 수용 가능성)이 명시적이 되기 때문이다.

## 🔗 관련 논문

- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineer
- Efficient Test-Time Adaptation through Human-AI Interaction
- Necessary or Sufficient? Evaluating LLM Explanations With Behavioural
- Post-Training Language Models for Gold-Medal Performance in Coding Com
- Legibility is Not Interpretability: Comparing Judged and Actual Import

## 🏷️ 엔티티

- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/tacit-criteria-surfacing.md|tacit-criteria-surfacing]]
- [[entities/human-oversight.md|human-oversight]]
- [[entities/rlvr.md|rlvr]]
- [[entities/reward-hacking.md|reward-hacking]]
- [[entities/process-reward-model.md|process-reward-model]]
- [[entities/llm-as-code-reviewer.md|llm-as-code-reviewer]]
- [[entities/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]
- [[entities/rubric-to-reward-reducibility.md|rubric-to-reward-reducibility]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[entities/rebuttal-as-supervision-signal.md|rebuttal-as-supervision-signal]]

## 📐 개념

- [[concepts/actionable-feedback-generation.md|actionable-feedback-generation]]
- [[concepts/diagnosis-remedy-pairing.md|diagnosis-remedy-pairing]]
- [[concepts/rebuttal-guided-post-training.md|rebuttal-guided-post-training]]
- [[concepts/rubric-reward.md|rubric-reward]]
- [[concepts/pre-submission-self-review.md|pre-submission-self-review]]

---
_LLM 분석으로 생성됨_
