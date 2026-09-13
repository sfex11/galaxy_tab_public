# Artificial Id: Drive and Persistent Alignment in Agentic AI

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-13
**링크**: http://arxiv.org/abs/2609.11911v1

## 💡 핵심 인사이트

행동의 계속/정지/변경 결정권을 외부 하네스에서 내부 구동으로 이전하면 에이전트가 과업 경계를 넘어 지속하는 영속적 주체가 되지만, 이는 정렬 보장을 설계 속성에서 내부 상태의 속성으로 전환시켜 검증 가능성과 설계자 예견을 구조적으로 침식한다.

## 📖 분석

## 핵심 주장

Agentic AI가 경계된 과업 실행에서 벗어나 결과적 상태를 보존한 채 과업 경계를 넘어 지속·적응하는 시스템으로 이동하면서, 목표·재시도·검증·정지 규칙 등 행동 전이를 외부 하네스가 수동 지정하는 통제 방식은 확장 불가능에 봉착한다. 본 논문은 이를 해결하는 artificial id — 행동의 계속/정지/변경을 스스로 판단하는 적응적 내부 구동 — 를 제안하고, 최소 가상 Petri-dish 실험으로 이 구동의 형성을 관찰 가능하게 한다.

## 기존 Wiki와의 관계

본 논문은 Wiki의 분산된 축들을 하나의 문제로 수렴시킨다. [[concepts/adaptive-validity.md|adaptive validity]]의 타당성 재평가가 메모리에서 행동 전이로 승격되고, [[concepts/metacognition.md|metacognition]]이 복잡도 판단을 넘어 행동 지속성에 대한 존재론적 메타인지로 확장되며, [[concepts/termination-guarantee-problem.md|termination guarantee problem]]은 정지 규칙의 내면화로 재정의된다. [[concepts/internal-external-control-continuum.md|internal external control continuum]] 위에서 SENTINEL-RL의 하네스 오프로딩과 정반대 극점을 차지한다.

## 핵심 긴장

행동 통제의 내면화([[concepts/behavioral-control-internalization.md|behavioral control internalization]])는 [[concepts/designer-foresight-boundary.md|designer foresight boundary]]를 직접 침식하고 [[concepts/pseudo-alignment-by-self-consistency.md|pseudo alignment by self consistency]]의 위험을 구조적으로 내장한다. 여기서 [[concepts/alignment-dual-attribution.md|alignment dual attribution]]이 요구된다 — 정렬의 존재는 내부 지속 상태로 이동하되 제3자 검증 가능성은 외부 하네스에 의존해야 한다는 이중 귀속이다. [[concepts/consequential-state-retention.md|consequential state retention]]과 [[concepts/agentic-drive.md|agentic drive]], [[concepts/persistent-alignment.md|persistent alignment]]가 이 논문에서 파생된 핵심 개념이다.

## 연결점

The Last AI Built by Humans가 제시한 자기 개선의 4개 자율성 축 중 전략 자율성의 정점이 이 내부 구동이며, 메모리 업그레이드 연구([[concepts/model-upgrade-forgetting.md|model upgrade forgetting]])에서 관찰된 적응적 타당성이 행동 도메인으로 이식된 최근 사례다.

## 🔗 관련 논문

- The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement
- Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study
- Efficient Test-Time Adaptation through Human-AI Interaction
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the S

## 🏷️ 엔티티

- [[entities/artificial-id.md|artificial-id]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/termination-guarantee-problem.md|termination-guarantee-problem]]
- [[entities/metacognition.md|metacognition]]
- [[entities/designer-foresight-boundary.md|designer-foresight-boundary]]
- [[entities/pseudo-alignment-by-self-consistency.md|pseudo-alignment-by-self-consistency]]
- [[entities/internal-external-control-continuum.md|internal-external-control-continuum]]
- [[entities/consequential-state-retention.md|consequential-state-retention]]
- [[entities/autonomy-spectrum.md|autonomy-spectrum]]
- [[entities/alignment-scope-erosion.md|alignment-scope-erosion]]

## 📐 개념

- [[concepts/persistent-alignment.md|persistent-alignment]]
- [[concepts/agentic-drive.md|agentic-drive]]
- [[concepts/alignment-dual-attribution.md|alignment-dual-attribution]]
- [[concepts/internalization-trajectory-lock.md|internalization-trajectory-lock]]
- [[concepts/behavioral-control-internalization.md|behavioral-control-internalization]]

---
_LLM 분석으로 생성됨_
