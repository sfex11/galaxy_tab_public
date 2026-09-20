# StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks via Agentic Distillation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20791v1

## 💡 핵심 인사이트

계층적 플래닝의 병목은 목표 분해가 아니라 스킬 전환 판정이며, VLM의 강한 추론조차 그 결정 경계가 과제 완료 기준과 미정렬되어 있어 증류를 통한 경계 정렬이 필수적이다.

## 📖 분석

StageGuard는 계층적 플래닝([[hierarchical-planning]])의 최약 고리가 상위 목표 분해가 아니라 '현재 스킬을 언제 종료하고 다음 서브태스크로 전환할 것인가'라는 전이 판정임을 규명한다. 기존 접근이 사전 설계된 완료 신호 체커에 의존하지만 이는 실세계 실행에서 획듍이 어렵다는 이중 문제를 지적한다.

핵심 기여는 agentic distillation이다. VLM은 강한 추론 능력을 갖지만 그 결정 경계가 과제 완료 기준과 본질적으로 정렬되어 있지 않다는 진단에서 출발하여, VLM의 전이 판단을 경량 정책으로 증류한다. [[knowledge-distillation]]이 능력 전이였다면 본 논문은 '판단 경계-과제 기준의 정렬'을 증류 대상으로 삼는 새 축을 연다.

구조적으로는 [[thought-action-separation]]의 역할 세분화다. 사고 계층(VLM)을 저빈도 고수준 전환 판단에만 배치하고 고빈도 저수준 제어는 학습된 전이 계층이 담당함으로써, [[skill-termination-judgment]]이 별도의 학습 가능한 능력으로 격상된다. 이는 Artificial Id 계열의 '계속/정지/전환' 메타 판단([[metacognition]])과 물리 행동 도메인에서 수렴한다.

또한 VLM 감독이 모든 스텝이 아닌 전이 지점에만 요구됨은 저빈도 고수준 감독으로 장기 과제의 프로세스 신호([[reward-sparsity]])를 구성할 수 있음을 시사하며, 언어적 완료 보고 대신 학습된 판정기가 신뢰 가능한 상태 전이 신호를 제공한다는 점에서 [[state-transition-anchored-reward]] 논의와 연결된다.

## 🔗 관련 논문

- StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks via Agentic Distillation

## 🏷️ 엔티티

- [[entities/stageguard.md|stageguard]]
- [[entities/agentic-distillation.md|agentic-distillation]]
- [[entities/stage-transition-learning.md|stage-transition-learning]]
- [[entities/skill-termination-judgment.md|skill-termination-judgment]]
- [[entities/hierarchical-planning.md|hierarchical-planning]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/metacognition.md|metacognition]]

## 📐 개념

- [[concepts/completion-signal-checker.md|completion-signal-checker]]
- [[concepts/decision-boundary-misalignment.md|decision-boundary-misalignment]]
- [[concepts/low-frequency-transition-supervision.md|low-frequency-transition-supervision]]
- [[concepts/agentic-distillation.md|agentic-distillation]]
- [[concepts/thought-action-separation.md|thought-action-separation]]

---
_LLM 분석으로 생성됨_
