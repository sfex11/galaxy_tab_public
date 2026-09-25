# Talk2Escape: Conversational Grounding for Vision-and-Language Navigation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28296v1

## 💡 핵심 인사이트

에이전트가 자신의 불확실성을 감지해 능동적으로 대화로 복구를 요청하는 '탈출 해치'는, 오류 누적에 취약한 개방형 루프 내비게이션을 인간-에이전트 통신으로 폐쇄하는 새로운 복구 프리미티브다.

## 📖 분석

Talk2Escape는 VLN의 단일 턴 개방형(open-loop) 패러다임 취약성을 진단하고, 대화적 그라운딩을 오류 복구 프리미티브로 도입한다. 지각 모호성·센서 노이즈·오도메트리 드리프트([[course-drift]])의 미세 편차 누적이 치명적 임무 실패로 귀결되는 문제는 [[compounding-error]]의 체화 내비게이션 발현이며, '내장된 복구 메커니즘 부재'는 [[unrecoverable-reasoning-error]]의 물리 도메인 실례다.

Three-Step Nav가 제로샷 VLN의 경로 이탈·조기 정지라는 구조적 실패를 진단했다면, 본 논문은 그 처방 측을 제공한다 — 에이전트가 자신의 불확실성을 감지하면 능동적으로 대화를 개시해 방향을 재확정하는 '탈출 해치'다. 이는 [[human-oversight]]를 상시 감독에서 온디맨드 유발로 전환하고, [[metacognition]](불확실성 자가 감지)이 도움 요청의 트리거가 되는 구조를 만든다. 언제 물을지는 [[expected-value-of-information]]의 체화 도메인 확장이며, 무엇을 물을지는 [[communication-access-planning-gap]]의 질문 생성 능력 문제다.

개방형 루프의 대화적 폐쇄는 [[closed-loop-training]] 계열과 공명하며, 통신이 조율 비용이 아니라 실패로부터의 복구 자원으로 재정의됨을 보여준다는 점에서 기존 통신 비용 중심 논의에 긍정적 극점을 추가한다.

## 🔗 관련 논문

- Three-Step Nav: A Hierarchical Global-Local Planner for Zero
- SafetyALFRED: Evaluating Safety-Conscious Planning of Multim

## 🏷️ 엔티티

- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/three-step-nav.md|three-step-nav]]
- [[entities/compounding-error.md|compounding-error]]
- [[entities/unrecoverable-reasoning-error.md|unrecoverable-reasoning-error]]
- [[entities/course-drift.md|course-drift]]
- [[entities/human-oversight.md|human-oversight]]
- [[entities/metacognition.md|metacognition]]
- [[entities/expected-value-of-information.md|expected-value-of-information]]
- [[entities/communication-access-planning-gap.md|communication-access-planning-gap]]
- [[entities/conversational-grounding.md|conversational-grounding]]

## 📐 개념

- [[concepts/open-loop-vulnerability.md|open-loop-vulnerability]]
- [[concepts/proactive-help-seeking.md|proactive-help-seeking]]
- [[concepts/dialogue-as-recovery-primitive.md|dialogue-as-recovery-primitive]]

---
_LLM 분석으로 생성됨_
