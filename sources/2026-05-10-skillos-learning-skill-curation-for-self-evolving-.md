# SkillOS: Learning Skill Curation for Self-Evolving Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-10
**링크**: http://arxiv.org/abs/2605.06614v1

## 💡 핵심 인사이트

스킬 큐레이션을 수동/휴리스틱 프로세스에서 학습 가능한 정책으로 전환함으로써, 에이전트의 자가 진화가 고정된 연산 집합의 조합을 넘어 큐레이션 전략 자체의 적응적 개선을 달성한다.

## 📖 분석

# SkillOS

**카테고리**: AI/ML — 에이전트 자가 진화
**생성일**: 2026-05-10

## 정의

SkillOS는 LLM 기반 에이전트가 스트리밍 태스크 수행 과정에서 경험으로부터 재사용 가능한 스킬을 증류하고, 이 스킬의 큐레이션(curration) 자체를 학습 가능한 과정으로 형식화하는 자가 진화 프레임워크다.

## 기존 Wiki와의 관계

기존 `granularity-based-skill-organization`이 스킬을 도메인이 아닌 세분화 수준(task-level, step-level)으로 조직해야 한다는 **설계 원칙**을 제시했다면, SkillOS는 이 큐레이션 과정 자체를 에이전트가 **학습하는 대상**으로 격상시킨다. 수동 큐레이션·경험적 휴리스틱·단기_horizon 훈련에 머물던 기존 접근법의 한계를, 스킬 연산을 모델이 내재화하도록 훈련하는 경로로 해결한다.

`experience-reuse` 엔티티는 재사용 가능성을 전제로만 다루었으나, SkillOS는 '어떤 경험을 스킬로 승격시킬 것인가'라는 **선택 문제**를 학습 가능한 결정으로 구체화한다. 이는 `self-improving-agent`의 자가 개선 경로를 '추론 체인 합성'에서 '스킬 생태계 구축'으로 확장한다.

## 핵심 기여

스킬 큐레이션을 고정된 연산 집합이 아닌 학습 가능한 정책으로 재정의함으로써, `internalization-of-tool-use`가 목표로 삼는 '외부 도구 의존성 극복'에 대한 구체적 메커니즘을 제공한다. 에이전트가 자신의 재귀적 복제본을 내부적 도구로 사용하는 패러다임에서, 스킬은 도구와 에이전트 사이의 중간 추상화 계층으로 기능한다.

## 관련 논문

- [[sources/2026-05-09-skillos-learning-skill-curation-for-self-evolving-.md|SkillOS: Learning Skill Curation for Self-Evolving Agents]]

## 🔗 관련 논문

- 2026 05 09 skillos learning skill curation for self evolving 

## 🏷️ 엔티티

- [[entities/skillos.md|skillos]]
- [[entities/llm-agent.md|llm-agent]]
- [[entities/experience-reuse.md|experience-reuse]]
- [[entities/self-improving-agent.md|self-improving-agent]]

## 📐 개념

- [[concepts/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[concepts/learnable-skill-operations.md|learnable-skill-operations]]
- [[concepts/skill-lifecycle-management.md|skill-lifecycle-management]]

---
_LLM 분석으로 생성됨_
