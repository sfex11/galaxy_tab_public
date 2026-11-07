# ReproBridge: Building Reproducibility into ML Research Artifacts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-07
**링크**: http://arxiv.org/abs/2611.08452v1

## 💡 핵심 인사이트

ML 재현의 실제 병목은 에이전트의 복구 능력 그 자체가 아니라 매 재현마다 소멸되는 복구 노동의 휘발성이며, 복구된 절차와 결정을 아티팩트에 영속화하면 재현성이 개별 에이전트의 능력 문제에서 에이전트 간 지식 이양의 누적 문제로 전환된다.

## 📖 분석

# ReproBridge: ML 연구 아티팩트에 재현성 내장 (2026-11-07)

**핵심 주장**: ML 실험 재현은 논문·공개 코드·부속 아티팩트에 산재한 정보로 절차를 재구성해야 하므로, 코딩 에이전트의 재현 성공은 공개 아티팩트 자체보다 '결측 세부를 채우는 병목 복구 능력'에 의존한다. ReproBridge는 정제된 코드베이스, 환경, 그리고 에이전트가 회복한 절차와 결정을 포함하는 표준화된 아티팩트 설계를 정의하고, 선행 에이전트의 복구 산출물을 보존하면 후속 독립 재현이 개선됨을 검증한다.

**Wiki와의 관계**:
- [[scientific-finding-reproducibility]]: 코딩 에이전트의 재현 '가능성'을 보인 선행 연구(sources/2026-05-05-can-coding-agents-reproduce-findings-in-computatio.md) 위에서, 재현 성패가 에이전트 능력이 아니라 복구 산출물의 영속성에 조건부임을 보여 질문을 심화한다.
- [[specification-incompleteness-propagation]]: 불완전 명세의 하류 전파를 반복 복구가 아닌 '1회 복구 + 아티팩트 고정'으로 수렴시키는 해법 측을 제공한다. IdeaAMBIG가 구현 결손을 측정했다면 본 논문은 결손을 채운 노동의 보존 경로를 연다.
- [[experience-reuse]]·[[validated-skill-library]]: 궤적·스킬·환경에 이어 '복구된 절차'가 제4의 재사용 단위가 된다 — 한 에이전트의 복구 노동이 아티팩트를 매개로 다음 에이전트의 자산이 되는 재현 노동의 복리화 구조.
- [[document-centric-research-infrastructure]]·[[intern-atlas]]: 아티팩트가 방법론 추적뿐 아니라 재현 절차의 운반체로 기능함을 재확인하며, 연구 인프라의 일급 소비자에 '재현 에이전트'를 추가한다.
- [[artifact-bound-optimization]]: 아티팩트가 성능 목표가 아닌 후속 재현 성공을 결정하는 축적 단위로 재정의된다.

**핵심 통찰**: 재현성을 에이전트 능력 문제가 아니라 복구 노동의 영속화 문제로 재정의한다 — 병목은 아티팩트의 결손 그 자체가 아니라, 매 재현마다 소멸되는 복구 노동에 있다.

## 🔗 관련 논문

- Can Coding Agents Reproduce Findings in Computational Materials Science
- Intern-Atlas: A Methodological Evolution Graph as Research Infrastructure
- Design Docs Are All You Need: An AI-native Machine-Learning Performance Regeneration
- IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research Ideas
- From Research Question to Scientific Workflow: Leveraging Agentic AI

## 🏷️ 엔티티

- [[entities/reprobridge.md|reprobridge]]
- [[entities/scientific-finding-reproducibility.md|scientific-finding-reproducibility]]
- [[entities/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[entities/specification-incompleteness-propagation.md|specification-incompleteness-propagation]]
- [[entities/document-centric-research-infrastructure.md|document-centric-research-infrastructure]]
- [[entities/artifact-bound-optimization.md|artifact-bound-optimization]]
- [[entities/experience-reuse.md|experience-reuse]]

## 📐 개념

- [[concepts/recovered-procedure-preservation.md|recovered-procedure-preservation]]
- [[concepts/standardized-artifact-design.md|standardized-artifact-design]]
- [[concepts/reproduction-work-compounding.md|reproduction-work-compounding]]

---
_LLM 분석으로 생성됨_
