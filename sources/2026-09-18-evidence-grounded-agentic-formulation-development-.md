# Evidence-Grounded Agentic Formulation Development in an Autonomous Laboratory

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19099v1

## 💡 핵심 인사이트

물리 자동 실험실이 모델과 독립적인 외부 검증자로 작동할 때, 구조화된 실험 증거에 근거한 LLM 에이전트 추론이 통계적 획득 함수를 대체해 실험 설계를 주도할 수 있다.

## 📖 분석

# Evidence-Grounded Agentic Formulation Development in an Autonomous Laboratory (2026-09-18)

난용성 약물의 경구 생체이용률을 높이는 SEDDS 제형 개발을 자동화하는 에이전트 시스템 **Andromeda 2**를 제시한다. 구조화된 자체 실험 증거에 대해 추론하고 계산·실험 도구를 호출해 제형 배치를 연속 설계·실행하며, 미니어처 자동 실험실에서 동일 예산의 확률론적 기저(Andromeda 1)와 비교된다.

## Wiki에서의 위치

[[entities/scientific-workflow-agent.md|scientific workflow agent]]와 [[concepts/autoresearch.md|autoresearch]] 논의를 물리 실험 영역으로 확장한다. 기존 워크플로우 에이전트가 명세 번역·실행에 집중했다면(Avatar), 본 논문은 실행 중 축적된 증거가 차기 배치 설계를 재정의하는 적응형 루프를 보여준다. [[concepts/evidence-grounded-diagnosis.md|evidence grounded diagnosis]]의 증거 기반 추론이 진단(증상→원인)에서 설계(증거→차기 실험)로 축 이동한 사례이며, [[concepts/exploratory-research-agent.md|exploratory research agent]] 계열에 물리 실험 루프 실례를 추가한다.

## 핵심 통찰

자동 실험실은 [[concepts/verification-as-system-external-relation.md|verification as system external relation]]의 이상적 실현이다 — 제형 성능은 모델과 무관한 물리 측정으로 심판되므로 자기 일관성 함정이 작동하지 않는다. 동일 예산 비교 설계는 [[concepts/cost-aware-agent-evaluation.md|cost aware agent evaluation]]의 구현으로, "에이전트 추론이 통계적 획득 함수를 대체할 수 있는가"를 비용 조건부로 정식화한다.

## 🔗 관련 논문

- Avatar: Toward Autonomous End-to-End Orchestration of Scientific Workf
- From Research Question to Scientific Workflow: Leveraging Agentic AI f
- HypoEvolve: Genetic Algorithms Enable Multi-Agent LLMs to Discover Sci
- Large Language Models (LLMs) for Telecom Root Cause Analysis (RCA): A
- SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Interpretabi

## 🏷️ 엔티티

- [[entities/autonomous-laboratory-agent.md|autonomous-laboratory-agent]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/evidence-grounded-diagnosis.md|evidence-grounded-diagnosis]]
- [[entities/exploratory-research-agent.md|exploratory-research-agent]]

## 📐 개념

- [[concepts/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[concepts/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]
- [[concepts/evidence-grounded-experiment-design.md|evidence-grounded-experiment-design]]
- [[concepts/expected-value-of-information.md|expected-value-of-information]]
- [[concepts/raw-evidence-anchoring.md|raw-evidence-anchoring]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-17-evaluating-verified-autonomy-in-quantum-engineerin]]: 물리적 자동 실험실이 모델과 독립된 외부 검증자로 작동할 때 에이전트 추론이 실험 설계를 주도할 수 있음을 양자 공학과 제형 개발에서 각각 보여준다.
