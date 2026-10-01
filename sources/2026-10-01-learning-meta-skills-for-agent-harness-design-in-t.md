# Learning Meta-Skills for Agent Harness Design in Test-Time AI4AI

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38143v1

## 💡 핵심 인사이트

개선을 가중치가 아닌 학습된 환경 구축 원칙(Meta-Skill)으로 매개하면 개선의 수행자(Builder)와 수혜자(Target)를 분리할 수 있으며, 하네스 설계 경험 자체가 재사용 가능한 지능 자산이 된다.

## 📖 분석

가중치 고정 하에서 Builder 에이전트가 Target 에이전트의 실행 환경(하네스)을 학습적으로 구축하는 test-time AI-for-AI 패러다임을 제시한다. 핵심은 Meta-Skill이다 — '언제 지원이 필요한가, 어떤 자원을 제공할 것인가'를 규정하는 재사용 가능한 원칙으로, Builder가 Target의 dev set 실행 피드백에서 학습하여 환경 구축 경험을 지식 자산화한다.

Wiki의 하네스 학습 계보에 '구축 주체의 분리'라는 새 축을 추가한다. [[harness-learning]]이 에이전트 자신의 하네스를 학습했다면, 본 논문은 별도 Builder가 Target을 위한 환경을 구축한다. 이는 [[harness-as-nonparametric-policy-layer]]가 규정한 '가중치 없이 피드백으로부터 학습되는 제2 정책 계층'의 위임형 실현이며, [[failure-guided-harness-growth]]·[[growing-harness]]의 자기 지향적 성장과 달리 성장 수행자가 타자 지향으로 전환된다.

[[improvement-autonomy-taxonomy]]의 [[environment-adaptation-autonomy]] 축에 위임형 변형을 제공하고, Meta-Skill은 [[skill-as-external-state]]의 대상을 실행 스킬에서 환경 구축 원칙으로 확장한다. [[agent-environment-generation]]에 생성기 자체가 개선되는 2차 학습 루프를, [[harness-as-capability-translator]]에 '번역 규칙의 학습 가능성'이라는 심화를 부여한다.

## 🔗 관련 논문

- Harness Learning Enables Generalizable Test-Time Adaptation
- Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Harness
- The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement
- CodeMidas: Scaling Agentic Coding RL Environments from Code Itself

## 🏷️ 엔티티

- [[entities/harness-learning.md|harness-learning]]
- [[entities/harness-as-nonparametric-policy-layer.md|harness-as-nonparametric-policy-layer]]
- [[entities/failure-guided-harness-growth.md|failure-guided-harness-growth]]
- [[entities/growing-harness.md|growing-harness]]
- [[entities/environment-adaptation-autonomy.md|environment-adaptation-autonomy]]
- [[entities/improvement-autonomy-taxonomy.md|improvement-autonomy-taxonomy]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/harness-as-capability-translator.md|harness-as-capability-translator]]
- [[entities/retraining-free-adaptation.md|retraining-free-adaptation]]
- [[entities/meta-harness-policy.md|meta-harness-policy]]
- [[entities/designer-foresight-boundary.md|designer-foresight-boundary]]
- [[entities/meta-learning.md|meta-learning]]
- [[entities/test-time-ai4ai.md|test-time-ai4ai]]
- [[entities/builder-target-separation.md|builder-target-separation]]
- [[entities/meta-skill.md|meta-skill]]

## 📐 개념

- [[concepts/test-time-ai4ai.md|test-time-ai4ai]]
- [[concepts/meta-skill.md|meta-skill]]
- [[concepts/builder-target-separation.md|builder-target-separation]]
- [[concepts/delegated-environment-adaptation.md|delegated-environment-adaptation]]

---
_LLM 분석으로 생성됨_
