# CodeMidas: Scaling Agentic Coding RL Environments from Code Itself

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.22068v1

## 💡 핵심 인사이트

코딩 RL 환경 스케일링의 병목은 코드 공급이 아니라 추출 원천의 선택이며, 개발 과정의 아티팩트(이슈·커밋)보다 제품(소스 코드의 구현된 기능)이 더 조밀하고 확장 가능한 환경 원시자원이다.

## 📖 분석

CodeMidas는 오픈소스 코드베이스의 구현된 기능을 실행 가능한 RL 환경으로 변환하는 에이전틱 파이프라인이다. 기존 방법이 이슈·커밋 같은 개발 아티팩트에 의존해 추출 가능한 태스크 범위가 제한되었던 반면, 소스 코드 자체를 1차 자원으로 삼아 환경 공급의 확장 축을 재정의한다.

[[environment-as-training-primitive]]의 코딩 도메인 실현이다. Terminal-Universe([[terminal-universe]])가 에이전트 궤적(경험)을 환경으로 재질의했다면, 본 논문은 외부 코드베이스(산출물)를 환경으로 변환하여 '환경 유래 자원'의 경험-산출물 양축을 완성한다. [[codebase-as-learning-environment]] 관점에서 ScienceIDE가 과학 코드베이스를 학습 환경화했다면, 본 논문은 범용 코딩 RL로 확장하며 '구현된 기능 = 태스크'라는 추출 단위를 확립한다.

[[rlvr]]의 전제인 신뢰할 수 있는 검증자를 갖춘 태스크 공급 문제를 코드베이스 자체에서 충족한다. 검증 가능성이 외부 벤치마크가 아닌 코드의 실행 의미론에서 유래함을 보여주며, [[environment-absence-bottleneck]]에 대한 공급 측 해법이기도 하다.

핵심 통찰: 개발 아티팩트는 개발 과정의 부수 기록일 뿐 코드 기능의 축소 표현이다. 환경 스케일링의 병목은 코드 공급이 아니라 추출 원천의 선택이며, 제품(코드)이 과정(아티팩트)보다 조밀한 [[experience-infrastructuralization]] 대상임을 실증한다.

## 🔗 관련 논문

- ScienceIDE: Turning World's Scientific Codebase into Agent L
- Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E
- Environment Evolution for Terminal Agents
- CUA-Universe: A Scalable and Dynamic Environment for Hybrid

## 🏷️ 엔티티

- [[entities/environment-as-training-primitive.md|environment-as-training-primitive]]
- [[entities/codebase-as-learning-environment.md|codebase-as-learning-environment]]
- [[entities/rlvr.md|rlvr]]
- [[entities/environment-absence-bottleneck.md|environment-absence-bottleneck]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/terminal-universe.md|terminal-universe]]
- [[entities/experience-infrastructuralization.md|experience-infrastructuralization]]
- [[entities/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[entities/pre-existing-data-assumption.md|pre-existing-data-assumption]]
- [[entities/environment-diversity-layered-guarantee.md|environment-diversity-layered-guarantee]]

## 📐 개념

- [[concepts/code-functionality-as-task-unit.md|code-functionality-as-task-unit]]
- [[concepts/product-over-process-environment-derivation.md|product-over-process-environment-derivation]]
- [[concepts/environment-supply-scaling.md|environment-supply-scaling]]
- [[concepts/artifact-vs-product-extraction-source.md|artifact-vs-product-extraction-source]]

---
_LLM 분석으로 생성됨_
