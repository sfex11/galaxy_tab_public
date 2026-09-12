# Artificial Id: Drive and Persistent Alignment in Agentic AI

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11911v1

## 💡 핵심 인사이트

행동의 계속·정지·변경을 결정하는 제어 기능을 외부 하네스의 명세에서 에이전트 내부의 적응적 구동체로 이전함으로써, 에이전트 제어의 근본 위상을 외부 규범에서 내부 본능으로 역전시킨다.

## 📖 분석

본 논문은 에이전트 제어의 근본 위상을 역전시킨다. 목표·재시도·검증·정지 규칙 등 행동 전이를 외부 하네스가 '손으로' 명세하는 현행 패러다임([[agentic-harness-engineering]])에 대해, 계속/정지/변경을 판단하는 적응적 내부 구동체 artificial id를 제안한다. Freud적 은유로 읽으면 통제가 하네스 계층(외부 초자아)에서 에이전트 내부 본능 계층으로 이동하는 것이다.

기존 Wiki와의 관계: (1) [[harness-native-training]]과 반대 방향인 '내부-네이티브 제어' 축을 연다. (2) [[termination-guarantee-problem]]의 정지 규칙을 외부 명세에서 내부 구동으로 재배치한다. (3) [[interpretive-vs-structural-enforcement]]의 해석적 강제를 넘어 규칙의 생성·적용 자체가 내부화된 제3 범주를 연다. (4) task 경계를 넘어 consequential state를 유지한다는 전제는 [[episodic-persistent-state-gap]]의 해소 방향을 제시한다. (5) 계속/변경 판단은 [[goal-fixation-meta-decision]]을 내부 구동으로 조작화한 것이다.

위험 축: 내부 구동의 자기 판단은 [[pseudo-alignment-by-self-consistency]]와 [[designer-foresight-boundary]]의 침식을 구조적으로 수반하며, 'Persistent Alignment'라는 표제는 정렬이 세션 경계를 넘어 유지되어야 한다는 [[alignment-scope-erosion]]의 새 국면을 시사한다. Petri-dish 최소 실험은 [[metacognition]]적 판단의 형성 과정을 외부 관측 가능하게 하는 방법론적 장치이며, [[autonomy-spectrum]]의 반성적 단계 구현 후보로 위치한다.

## 🔗 관련 논문

- Procedural Graphs: Self-Evolving Execution Structures for LLM Agents
- Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Mo
- Avatar: Toward Autonomous End-to-End Orchestration of Scient

## 🏷️ 엔티티

- [[entities/artificial-id.md|artificial-id]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/termination-guarantee-problem.md|termination-guarantee-problem]]
- [[entities/metacognition.md|metacognition]]
- [[entities/interpretive-vs-structural-enforcement.md|interpretive-vs-structural-enforcement]]
- [[entities/episodic-persistent-state-gap.md|episodic-persistent-state-gap]]
- [[entities/alignment-scope-erosion.md|alignment-scope-erosion]]
- [[entities/designer-foresight-boundary.md|designer-foresight-boundary]]
- [[entities/pseudo-alignment-by-self-consistency.md|pseudo-alignment-by-self-consistency]]
- [[entities/goal-fixation-meta-decision.md|goal-fixation-meta-decision]]
- [[entities/autonomy-spectrum.md|autonomy-spectrum]]
- [[entities/adaptive-validity.md|adaptive-validity]]

## 📐 개념

- [[concepts/artificial-id.md|artificial-id]]
- [[concepts/behavioral-transition-internalization.md|behavioral-transition-internalization]]
- [[concepts/persistent-alignment.md|persistent-alignment]]
- [[concepts/consequential-state-retention.md|consequential-state-retention]]
- [[concepts/internal-external-control-continuum.md|internal-external-control-continuum]]

---
_LLM 분석으로 생성됨_
