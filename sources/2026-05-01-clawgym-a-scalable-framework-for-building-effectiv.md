# ClawGym: A Scalable Framework for Building Effective Claw Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26904v1

## 💡 핵심 인사이트

에이전트 하네스를 평가 관측치에서 훈련 가능한 일급 엔지니어링 객체로 승격시킴으로써, 샌드박스-실세계 격차를 훈련 데이터 합성 파이프라인을 통해 구조적으로 좁히는 최초의 통합 프레임워크를 제공한다.

## 📖 분석

# ClawGym

ClawGym은 Claw 스타일 개인 에이전트의 전체 생명주기—검증 가능한 학습 데이터 합성, 에이전트 학습 통합, 진단적 평가—를 지원하는 확장 가능한 프레임워크다. 기존 Wiki에서 OpenClaw 생태계는 **보안 평가** 중심으로만 분석되었고, ClawBench는 **평가 벤치마크**로만 기록되었으나, ClawGym은 이 둘 사이의 누락된 축—**체계적 개발 인프라**—를 최초로 제공한다.

이는 [[entities/harness-engineering.md|하네스 엔지니어링]]의 구체적 실현 사례로, [[concepts/harness-as-hidden-variable.md|하네스를 은닉 변수에서 일급 객체로 승격]]시킨다. 기존에 [[concepts/sandbox-liveworld-gap.md|샌드박스-실세계 격차]]로만 진단되던 문제에 대해, 검증 가능한 학습 데이터 합성을 통해 샌드박스 내 훈련 품질을 체계적으로 끌어올리는 경로를 제공한다. 또한 [[concepts/agent-environment-generation.md|에이전트 환경 생성]]을 벤치마크용 정적 환경에서 학습-평가 통합 파이프라인으로 확장하며, [[concepts/observability-driven-evolution.md|관측 가능성 주도 진화]]의 요구를 진단적 평가 기능으로 구현한다.

[[concepts/computer-use-agent.md|컴퓨터 사용 에이전트]] 연구가 단일 세션 성능 평가에서 정체되어 있던 상황에서, ClawGym은 훈련 데이터 합성→학습→진단의闭环을 제공하여 에이전트 개발을 공학적 파이프라인으로 전환한다.

## 🔗 관련 논문

- 2026-04-30-agentic-harness-engineering-observability-driven-a.md
- 2026-04-07-a-systematic-security-evaluation-of-openclaw-and-i.md
- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md
- 2026-04-09-gym-anything-turn-any-software-into-an-agent-envir.md

## 🏷️ 엔티티

- [[entities/clawgym.md|clawgym]]
- [[entities/openclaw.md|openclaw]]
- [[entities/harness-engineering.md|harness-engineering]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/observability-driven-evolution.md|observability-driven-evolution]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]

## 📐 개념

- [[concepts/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[concepts/full-lifecycle-agent-framework.md|full-lifecycle-agent-framework]]
- [[concepts/diagnostic-agent-evaluation.md|diagnostic-agent-evaluation]]
- [[concepts/persistent-workspace-training.md|persistent-workspace-training]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

