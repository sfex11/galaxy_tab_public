# Advancing Clinical Genomic Analysis with a Skill-Centred Agent

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40556v1

## 💡 핵심 인사이트

오류가 임상적으로 치명적인 도메인에서는 스킬 큐레이션의 주체가 학습에서 전문가로 이동하며, 전문가 지식의 실행 가능 단위 컴파일(105개 스킬)과 의존성 인지 조율이 에이전트 능력의 구조를 결정한다.

## 📖 분석

ClinGeX는 임상 유전체 분석을 위해 105개의 전문가 큐레이션 실행 가능 스킬을 태스크별 검색과 의존성 인지 오케스트레이션으로 조합하는 LLM 에이전트다. 본 논문은 스킬 중심 설계의 큐레이션 주체 축을 확정한다 — [[concepts/skill-curation-as-learning.md|skill curation as learning]]이 학습된 큐레이션으로 자기 개선을 추구하는 극점이라면, ClinGeX는 오류가 임상적으로 치명적인 도메인에서 큐레이션을 전문가에게 위임하는 상보 극점이다. 큐레이션 주체(학습 vs 전문가)가 스킬 중심 에이전트 설계의 새 선택 축이며, 그 선택이 도메인 위험 수준의 함수임을 실증한다.

세 가지 구조적 기여가 있다. 첫째, 전문가 지식을 실행 가능 단위로 컴파일하는 [[concepts/expert-curated-skill-library.md|expert curated skill library]]의 임상 실현 — 진화하는 가이드라인·데이터베이스 지식이 감사 가능한 소프트웨어 자산으로 축적되어 [[concepts/validated-skill-library.md|validated skill library]]의 임상 버전이 된다. 둘째, [[concepts/task-specific-skill-retrieval.md|task specific skill retrieval]]이 [[concepts/skill-existence-blindness.md|skill existence blindness]]를 해소한다 — 파라미터에 없는 스킬의 존재를 모델이 알 수 없는 한계를 스킬 공간 검색으로 완화한다. 셋째, [[concepts/dependency-aware-skill-orchestration.md|dependency aware skill orchestration]] — 다단계 유전체 분석에서 스킬 간 선후 관계가 실행 가능성을 결정하므로, 검색(선택)과 오케스트레이션(조율)이 독립 설계 변수로 분해됨을 [[concepts/skill-selection-functional-split.md|skill selection functional split]]과 함께 확정한다.

[[entities/skillos.md|skillos]]와의 대비가 핵심 맥락이다. SkillOS가 스킬 큐레이션 자체를 학습 대상으로 삼았다면, ClinGeX는 임상 도메인의 검증 불가능성 때문에 큐레이션·검증 주체를 전문가로 고정한다. 이는 자기 개선 에이전트의 큐레이션이 보편 해법이 아니라 도메인 위험에 조건부임을 보여주며, [[concepts/medical-ai.md|medical ai]]의 스코프를 근거 생성에서 전문 지식의 스킬화로 확장한다.

## 🔗 관련 논문

- SkillOS: Learning Skill Curation for Self-Evolving Agents
- A Living Benchmark for Information Retrieval from Electronic Health Records
- Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable

## 🏷️ 엔티티

- [[entities/clingex.md|clingex]]
- [[entities/skill-selection-functional-split.md|skill-selection-functional-split]]
- [[entities/validated-skill-library.md|validated-skill-library]]
- [[entities/skillos.md|skillos]]
- [[entities/medical-ai.md|medical-ai]]
- [[entities/skill-existence-blindness.md|skill-existence-blindness]]
- [[entities/dependency-aware-skill-orchestration.md|dependency-aware-skill-orchestration]]
- [[entities/task-specific-skill-retrieval.md|task-specific-skill-retrieval]]

## 📐 개념

- [[concepts/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[concepts/expert-curated-skill-library.md|expert-curated-skill-library]]

---
_LLM 분석으로 생성됨_
