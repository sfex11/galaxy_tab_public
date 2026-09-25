# Agent-Editing World Model: Rethinking World Modeling for LLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-25
**링크**: http://arxiv.org/abs/2609.28416v1

## 💡 핵심 인사이트

세계 모델의 가치는 환경 예측 정확도가 아니라, 실제 피드백이 가용한 조건에서 오염된 에이전트 태스크 상태(미지원 가정·낡은 계획)를 정제하는 개입 능력에 있다.

## 📖 분석

## Agent-Editing World Model: 세계 모델링의 역할 재정의

본 논문은 언어 세계 모델의 전제를 공격한다. 기존 세계 모델은 환경 관찰을 예측·재구성했으나, 고엔트로피·실행 의존적 도구 응답은 실제 피드백이 가용한 상황에서 예측 가치가 제한적이라는 진단이다. 대신 세계 모델의 산출 대상을 환경이 아닌 **에이전트의 태스크 상태**로 전환한다 — 미지원 가정과 낡은 계획이 히스토리에 지속되어 추론을 오염시키는 wiki:task-state-contamination을 세계 모델이 편집·정제하는 패러다임이다.

### 기존 Wiki와의 관계

**세계 모델 산출 형식 치환의 제3 사례**: wiki:world-model-output-format-substitution 계열의 확장이다. 판별적 세계 모델이 상태 공간 → 행동-가치 공간으로 형식을 바꿨다면, 본 논문은 환경 예측 → 에이전트 상태 개입으로 이동시켜, 세계 모델링 연구의 관심이 '환경을 얼마나 잘 시뮬레이션하는가'에서 '에이전트 내부 상태를 얼마나 잘 교정하는가'로 이동하는 흐름을 확정한다. wiki:world-model-in-pieces의 특수화 논의와 결합하면, 세계 모델의 피스 중 하나가 에이전트 자기 상태임이 드러난다.

**망각·오염 관리 계보와의 접속**: 태스크 상태 오염은 wiki:cumulative-memory-contamination의 태스크 내 발현이며, wiki:adaptive-validity이 예측한 't시점에 옳던 계획이 t+1에 무효가 되는' 구조의 실패 양상이다. wiki:task-conditioned-memory-clearance가 협력 게임 이론적 귀속으로 망각 기준을 정했다면, 본 논문은 세계 모델 기반 상태 편집이라는 제2의 정제 경로를 연다. 컨텍스트 차원에서는 wiki:non-selective-context-accumulation의 해법 축도 된다.

### 인사이트

세계 모델의 진짜 가치는 예측 정확도가 아니라, 피드백이 풍부한 환경에서 오염된 상태를 정제하는 개입 능력에 있다. '무엇을 예측할 것인가'가 아니라 '무엇을 편집할 것인가'가 세계 모델 설계의 새로운 1차 질문이 된다.

## 🔗 관련 논문

- Benchmarking World Models for Continual Learning on Compositional Tasks
- Discriminative World Models for Web Agents
- MeClear: Cooperative Game-Theoretic Attribution and Risk-Aware Forgetting
- CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents
- Artificial Id: Drive and Persistent Alignment in Agentic AI

## 🏷️ 엔티티

- [[entities/world-model.md|world-model]]
- [[entities/task-state-contamination.md|task-state-contamination]]
- [[entities/agent-editing-world-model.md|agent-editing-world-model]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/world-model-output-format-substitution.md|world-model-output-format-substitution]]
- [[entities/cumulative-memory-contamination.md|cumulative-memory-contamination]]
- [[entities/task-conditioned-memory-clearance.md|task-conditioned-memory-clearance]]
- [[entities/non-selective-context-accumulation.md|non-selective-context-accumulation]]

## 📐 개념

- [[concepts/world-model.md|world-model]]
- [[concepts/task-state-contamination.md|task-state-contamination]]
- [[concepts/agent-editing-world-model.md|agent-editing-world-model]]
- [[concepts/adaptive-validity.md|adaptive-validity]]
- [[concepts/world-model-output-format-substitution.md|world-model-output-format-substitution]]
- [[concepts/cumulative-memory-contamination.md|cumulative-memory-contamination]]
- [[concepts/task-conditioned-memory-clearance.md|task-conditioned-memory-clearance]]
- [[concepts/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[concepts/memory-management.md|memory-management]]

---
_LLM 분석으로 생성됨_
