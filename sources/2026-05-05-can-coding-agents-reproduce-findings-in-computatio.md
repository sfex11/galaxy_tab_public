# Can Coding Agents Reproduce Findings in Computational Materials Science?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00803v1

## 💡 핵심 인사이트

소프트웨어 엔지니어링 벤치마크에서의 코딩 에이전트 성공은 계산 과학 워크플로우로 자동 전이되지 않으며, 도메인 특화 절차 탐색과 과학적 맥락에서의 결과 해석이 별개의 능력 축으로 요구된다.

## 📖 분석

AutoMat은 소프트웨어 엔지니어링 벤치마크에서 입증된 코딩 에이전트의 강력한 성능이 계산 과학 워크플로우로 전이되는지를 검증하는 벤치마크다. 기존 [[entities/computer-use-agent|computer-use-agent]] 평가가 SE 태스크에 집중했다면, AutoMat은 코딩 능력뿐 아니라 도메인 특화 절차 탐색과 과학적 주장 맥락에서의 결과 해석이라는 추가 요구를 명시적으로 문제화한다. 이는 [[entities/sandbox-liveworld-gap|sandbox-liveworld-gap]]의 과학 도메인 인스턴스로 작동한다 — SE 샌드박스에서의 성공이 실제 과학적 재현 환경으로 전이되지 않을 수 있음을 구조화한다.

[[entities/autoresearch|autoresearch]]가 문헌 탐색에서 실행 워크플로우로 확장되었다면, AutoMat은 '발견 재현'이라는 과학적 검증 축을 추가한다. [[entities/scientific-workflow-agent|scientific-workflow-agent]]의 능력이 일반 코딩과 도메인 절차 내비게이션 사이에 구조적 간극이 존재함을 실증할 가능성이 높으며, 이는 [[entities/harness-as-hidden-variable|harness-as-hidden-variable]]이 과학 워크플로우에서 어떻게 현현하는지를 보여준다 — 과학적 하네스(시뮬레이션 파이프라인, 파라미터 설정, 결과 검증)가 태스크 난이도의 은닉 변수로 작동할 수 있다.

## 🔗 관련 논문

- 2026-05-01-clawgym-a-scalable-framework-for-building-effectiv.md
- 2026-05-02-claw-eval-live-a-live-agent-benchmark-for-evolving.md
- 2026-04-25-from-research-question-to-scientific-workflow-leve.md
- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md

## 🏷️ 엔티티

- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/benchmark.md|benchmark]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/harness-as-hidden-variable.md|harness-as-hidden-variable]]

## 📐 개념

- [[concepts/domain-procedure-navigation.md|domain-procedure-navigation]]
- [[concepts/scientific-finding-reproducibility.md|scientific-finding-reproducibility]]
- [[concepts/se-science-transfer-gap.md|se-science-transfer-gap]]

---
_LLM 분석으로 생성됨_
