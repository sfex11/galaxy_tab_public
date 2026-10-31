# Advancing Clinical Genomic Analysis with a Skill-Centred Agent

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-31
**링크**: http://arxiv.org/abs/2610.40556v1

## 💡 핵심 인사이트

급변하는 고위험 도메인(임상 유전체)에서는 능력을 전문가 큐레이션 스킬 라이브러리로 외부화하고 과제별 검색·의존성 인식 조합으로 운용하는 설계가 모델 내면화보다 유지보수 가능성과 감사 가능성을 동시에 제공한다.

## 📖 분석

## ClinGeX: 스킬 중심 임상 유전체 분석 에이전트

임상 유전체 분석은 급변하는 가이드라인·데이터베이스·계산 증거의 통합이 전문가 병목인 도메인이다. ClinGeX는 105개 전문가 큐레이션 실행 가능 스킬을 과제별 검색과 의존성 인식 오케스트레이션으로 조합하는 LLM 에이전트로, 능력을 모델 파라미터가 아닌 외부 스킬 라이브러리에 위치시키는 [[skill-as-external-state]] 원리의 최대 규모 임상 실현이다.

[[skill-curation-as-learning]]·[[skillos]] 계열이 자기 진화적 큐레이션을 다뤘다면, 본 논문은 큐레이션 권한을 임상 전문가에게 유지하는 상보 극점을 제시한다 — 고위험 도메인에서는 큐레이션 주체가 학습된 에이전트가 아닌 전문가여야 신뢰성과 규제 정합성이 확보된다. 105개 큐레이션 스킬은 [[validated-skill-library]]의 전문가 검증 버전이며, 과제별 스킬 검색은 [[expert-prior-retrieval]]의 '문서→실행 절차' 전환이다.

가이드라인의 지속 갱신은 스킬 타당성을 시간 조건부로 만들어 [[adaptive-validity]]의 임상 확장을 요구한다. [[clinical-graph-learning]] 계열이 보여준 임상 LLM 응용의 이동(데이터 구조 정제→전문가 절차 실행)을 확정하며, [[grounded-clinical-qa]]의 근거 인용이 실행 가능한 증거 통합 워크플로우로 진화하는 지점이기도 하다.

## 🔗 관련 논문

- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Designer-RSI: Evolving Procedural Memory from User Traffic for Agentic
- Skill-Space Shooting for Autonomous Robot Policy Improvement
- New LoRA Skills Should Read but Never Write
- Superintelligent Retrieval Agent: The Next Frontier of Infor
- LLM as Clinical Graph Structure Refiner: Enhancing Represent

## 🏷️ 엔티티

- [[entities/clingex.md|clingex]]
- [[entities/skill-as-external-state.md|skill-as-external-state]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[entities/skillos.md|skillos]]
- [[entities/skill-lifecycle-management.md|skill-lifecycle-management]]
- [[entities/expert-prior-retrieval.md|expert-prior-retrieval]]
- [[entities/skill-existence-blindness.md|skill-existence-blindness]]
- [[entities/skill-selection-functional-split.md|skill-selection-functional-split]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/medical-ai.md|medical-ai]]
- [[entities/clinical-graph-learning.md|clinical-graph-learning]]
- [[entities/grounded-clinical-qa.md|grounded-clinical-qa]]

## 📐 개념

- [[concepts/dependency-aware-skill-orchestration.md|dependency-aware-skill-orchestration]]
- [[concepts/task-specific-skill-retrieval.md|task-specific-skill-retrieval]]
- [[concepts/expert-curated-skill-library.md|expert-curated-skill-library]]

---
_LLM 분석으로 생성됨_
