# Strategist: Evolving Reasoning with Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03618v1

## 💡 핵심 인사이트

에이전트 시스템의 수작 절반(추론 전략)을 조합 가능한 코드 블루프린트의 진화 라이브러리로 전환하면, 전략 구축 경험이 태스크를 가로질러 복리로 누적될 수 있다.

## 📖 분석

모델은 에이전트 시스템의 절반에 불과하며, 나머지 절반인 추론 전략(모델 호출을 응답으로 조직하는 절차)은 현재 수작으로 작성되고 한 전략 구축 경험이 다음 태스크로 이월되지 않는다는 진단에서 출발한다. Strategist는 태스크를 가로질러 추론 전략을 진화시키는 메타-에이전트로, 전략을 블루프린트 — 다른 전략이 재사용 가능한 실행 코드 — 로 작성하고 이들이 라이브러리로 축적되게 한다.

기존 Wiki 대비 두 확장이 있다. 첫째, [[concepts/harness-learning.md|harness learning]] 계열([[concepts/meta-skill.md|meta skill]]의 Builder, Grow the Harness)이 태스크 내 하네스 성장을 다뤘다면 본 논문은 성장 단위를 '전략 코드'로 명시하고 태스크 간 이월을 구조의 핵심으로 삼는다. 둘째, [[concepts/skill-as-external-state.md|skill as external state]]와 [[concepts/validated-skill-library.md|validated skill library]]의 라이브러리 논리가 태스크 스킬에서 추론 전략으로 상향 확장되어, 전략 간 재사용이 코드 합성으로 실현된다. 이는 [[entities/system-scaling.md|system scaling]]의 모델-전략 이분법을 진화 가능한 자산 구조로 구체화한다.

핵심 통찰: 하네스 진화의 병목이 학습 방법이 아니라 재사용 단위의 부재라면, 전략을 조합 가능한 코드 아티팩트로 격상하는 것이 [[concepts/harness-scaling-axis.md|harness scaling axis]]의 복리 구조를 여는 경로다. [[concepts/meta-harness-policy.md|meta harness policy]]가 기존 전략의 '배정'이었다면 Strategist는 새 전략의 '작성·진화'로 계층이 한 단계 올라간다.

## 🔗 관련 논문

- Learning Meta-Skills for Agent Harness Design in Test-Time A
- Grow the Harness, Not the Context: From Strategy-Free Scaffo
- Harness Learning Enables Generalizable Test-Time Adaptation
- SkillOS: Learning Skill Curation for Self-Evolving Agents

## 🏷️ 엔티티

- [[entities/strategist.md|strategist]]
- [[entities/meta-skill.md|meta-skill]]
- [[entities/harness-learning.md|harness-learning]]
- [[entities/system-scaling.md|system-scaling]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/code-as-evolution-unit.md|code-as-evolution-unit]]
- [[entities/harness-scaling-axis.md|harness-scaling-axis]]
- [[entities/meta-harness-policy.md|meta-harness-policy]]

## 📐 개념

- [[concepts/strategy-blueprint-library.md|strategy-blueprint-library]]
- [[concepts/cross-task-strategy-carriage.md|cross-task-strategy-carriage]]
- [[concepts/inference-strategy-evolution.md|inference-strategy-evolution]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-05-mdskill-learning-to-internalize-skill-memory-throu]]: 태스크 경험의 축적·재사용이라는 공통 목표를 외부 전략 블루프린트 라이브러리(외재화)와 스킬 메모리의 증류적 내재화(내재화)라는 반대 방향의 경로로 추구한다.
- → [[sources/2026-11-06-compressionbench-how-can-your-coding-agents-compre]]: 재귀적 자기개선의 한 단계를 코딩 에이전트의 자율 모델 압축과 추론 전략 라이브러리의 복리 축적이라는 두 경로로 구현한다.
