# StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks via Agentic Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-19
**링크**: http://arxiv.org/abs/2609.20791v1

## 💡 핵심 인사이트

장기 로봇 태스크의 계층적 플래닝에서 실질 병목은 개별 스킬 능력이 아니라 '언제 스킬을 종료할 것인가'의 전이 판단이며, 이를 사전 설계 체커 대신 VLM 추론의 증류로 학습 가능한 문제로 전환할 수 있다.

## 📖 분석

StageGuard는 장기 로봇 태스크 계층적 플래닝의 핵심 병목 — '현재 스킬을 언제 종료하고 다음 서브태스크로 전환할 것인가'의 스테이지 전이 판단 — 을 학습 가능한 문제로 전환한다. 기존 접근이 사전 설계된 완료 신호 체커(실세계 획득 곤란)에 의존했다면, 본 논문은 VLM의 추론을 agentic distillation으로 전이 판별기에 증류하여, VLM 판단 경계가 태스크 완료 기준에 내재 정렬되지 않는 간극을 학습으로 봉합한다.

Wiki 지형에서 이 논문은 세 간선을 잇는다. (1) [[concepts/adaptive-transition-discovery.md|adaptive transition discovery]]가 훈련 데이터 생성에서 transition 이벤트의 적응적 발견을 다뤘다면, 본 논문은 실행 시점 스킬 전이 판단으로 확장하여 '경계는 주어지는 것이 아니라 발견되는 것'([[concepts/turn-as-derived-unit.md|turn as derived unit]])의 로봇 도메인 실현이다. (2) [[concepts/thought-action-separation.md|thought action separation]]의 분업을 세분화한다 — 사고 계층(VLM/판별기)이 행동 실행이 아니라 '행동 전환 판단'을 전담하면, VLM 추론이 실시간 제어 대신 저빈도 고수준 판단에 효율 배치된다. (3) [[entities/skill-conditioned-gating.md|skill conditioned gating]] 계열(The Router Within)이 스킬 '선택' 게이트를 다뤘다면, 본 논문은 스킬 '종료' 게이트라는 직교하는 지점을 공급한다.

이론적으로, 사전 설계 체커가 설계자 예견 경계([[concepts/designer-foresight-boundary.md|designer foresight boundary]])에 갇히는 문제를 VLM 증류가 완화하되, 증류 파이프라인 자체가 정렬을 만들어내는 하네스 설계 아티팩트([[concepts/elicitation-as-harness-artifact.md|elicitation as harness artifact]])가 되는 점, 그리고 '계속/정지/변경' 메타 판단([[concepts/metacognition.md|metacognition]], [[concepts/artificial-id.md|artificial id]])이 에이전트 전이 수준에서 스킬 전이라는 학습 가능한 저위험 단위로 국소화되는 점이 핵심 시사점이다.

## 🔗 관련 논문

- In-Context Robot Learning with VLM Agents (2026-09-18)
- The Router Within: Eliciting Native Skill Routing from a Frozen LLM (2026-09-16)
- Seeing Before Synthesizing: VLM-Guided Transition Event Discovery (2026-09-06)

## 🏷️ 엔티티

- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/adaptive-transition-discovery.md|adaptive-transition-discovery]]
- [[entities/turn-as-derived-unit.md|turn-as-derived-unit]]
- [[entities/skill-conditioned-gating.md|skill-conditioned-gating]]
- [[entities/designer-foresight-boundary.md|designer-foresight-boundary]]
- [[entities/elicitation-as-harness-artifact.md|elicitation-as-harness-artifact]]
- [[entities/local-sufficiency.md|local-sufficiency]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/metacognition.md|metacognition]]

## 📐 개념

- [[concepts/agentic-distillation.md|agentic-distillation]]
- [[concepts/stage-transition-learning.md|stage-transition-learning]]
- [[concepts/skill-termination-judgment.md|skill-termination-judgment]]

---
_LLM 분석으로 생성됨_
