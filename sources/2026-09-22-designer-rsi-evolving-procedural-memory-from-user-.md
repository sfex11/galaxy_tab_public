# Designer-RSI: Evolving Procedural Memory from User Traffic for Agentic Graphic Design

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22086v1

## 💡 핵심 인사이트

오라클이 없는 창작 도메인에서 자기 개선의 검증 신호를 모델 내부 판단 대신 사용자 트래픽에서 얻으면, 동결 모델의 감사 가능성을 유지한 채 외부 절차적 메모리 진화만으로 재귀적 자기 개선이 성립한다.

## 📖 분석

프로그래밍 오라클이 존재하지 않는 그래픽 디자인 도메인에서 재귀적 자기 개선을 실현한다. 동결된 프론티어 모델이 230개 이상의 도구로 전문 디자인 소프트웨어를 조작하고, 외부 절차적 메모리가 사용자 트래픽에서 재사용 가능한 디자인 절차(자연어 스킬)를 축적·정제한다.

이 구조는 [[bilevel-self-evolution]]의 창작 도메인 실현이다 — 태스크 수행(동결 모델)과 개선 절차(메모리 진화)가 분리되어 파라미터 변경 없이 지속적 능력 향상이 가능함을 보여준다. [[skill-as-external-state]] 관점에서 SkillOS 계열 스킬 큐레이션을 무오라클 도메인으로 확장하며, 스킬 정제가 시스템 능력의 유일한 진화 통로가 되는 극단적 외부화 사례다.

핵심 질문은 [[rlvr]]이 성립하지 않는 환경에서 개선 신호의 원천이다. 사용자 트래픽이 외부 앵커로 기능하여 [[circular-validity-problem]]을 회피한다 — 이는 [[human-trace-external-anchoring]] 원리의 자기 개선 도메인 적용이다. Learning to Coach가 코치 모듈에 개선을 위임했다면([[improvement-delegation]]), 본 논문은 위임 대상을 외부 메모리로 좁혀 동결 모델의 감사 가능성을 유지한다. 가중치 대신 자연어 스킬을 진화시키는 선택은 [[designer-foresight-boundary]]의 부분 완화이기도 하다 — 스킬 진화는 가중치 변화보다 검증·롤백이 용이하다.

## 🔗 관련 논문

- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Learning to Coach for Experiential Learning
- The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement
- PlayTrain: An Efficient Reinforcement Learning Framework for LLM-Gener

## 🏷️ 엔티티

- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/recursive-self-improvement.md|recursive-self-improvement]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/bilevel-self-evolution.md|bilevel-self-evolution]]
- [[entities/skill-lifecycle-management.md|skill-lifecycle-management]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/improvement-delegation.md|improvement-delegation]]
- [[entities/human-trace-external-anchoring.md|human-trace-external-anchoring]]
- [[entities/rlvr.md|rlvr]]
- [[entities/designer-foresight-boundary.md|designer-foresight-boundary]]

## 📐 개념

- [[concepts/continual-learning.md|continual-learning]]
- [[concepts/user-turn-generation.md|user-turn-generation]]
- [[concepts/experience-reuse.md|experience-reuse]]
- [[concepts/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[concepts/endogenous-self-evolution.md|endogenous-self-evolution]]

---
_LLM 분석으로 생성됨_
