# GEPA-Curator: Curated Learning for Self Improving Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37651v1

## 💡 핵심 인사이트

에이전틱 실패의 학습 가치는 원인 귀속에 의해 결정된다 — 프롬프트 약점이 아닌 하네스 한계·확률적 실행·잡음 judge에서 온 실패는 자기 개선 루프에 투입하면 오히려 유해하므로, 자기 개선의 핵심 병목은 학습 방법이 아니라 학습 태스크의 큐레이션에 있다.

## 📖 분석

# GEPA-Curator: Curated Learning for Self Improving Agents

## 핵심 주장
GEPA 계열 반사형 프롬프트 최적화기는 실패 롤아웃에서 학습하지만, 에이전틱 실패의 원인은 프롬프트 약점에 국한되지 않는다 — 하네스 한계, 확률적 실행, 잡음 많은 judge에서 비롯된 실패는 유용한 학습 신호가 없거나 오히려 유해하다. 따라서 자기 개선 루프 상류에 '어떤 태스크를 학습 재료로 제공할 것인가'를 선별하는 큐레이션 계층이 필수적이다.

## 기존 Wiki와의 관계

### failure-as-causal-data의 정교화
[[failure-as-causal-data]]가 실패를 인과 지식의 원료로 취급하는 패러다임을 제시했다면, 본 논문은 그 전제에 근본 단서를 단다 — 실패가 인과 데이터가 되려면 원인이 에이전트 측 학습 가능 요인에 귀속되어야 하며, 실패 원인 귀속(failure provenance)이 학습 가치의 판정 기준이 된다. [[forgetting-as-accumulation-quality-management]]가 축적 후 품질 관리를 다룬다면 본 논문은 유입 전 큐레이션을 다뤄, 경험 품질 관리의 양단을 완성한다.

### 평가 결함의 훈련 역류
잡음 judge를 유해 학습 요인으로 명시한 것은 [[black-box-instrument-drift]]·[[judge-instrument-reliability]] 계열의 평가 신뢰성 문제가 훈련 루프로 역류하는 경로를 확정한다. 하네스 한계를 실패 원인으로 꼽은 것은 [[harness-model-co-evolution]]에 '학습 전 하네스-모델 원인 분리'라는 새 전제를 부여한다.

### 자기 훈련 샘플링의 제3축
[[self-training-data-construction]]의 상류에 태스크 선택 계층을 추가한다. [[strategic-diversity]]가 다양성으로 샘플을 골랐다면 본 논문은 원인 귀속 가능성으로 골라, 자기 훈련 샘플링이 다양성·품질·귀속 가능성의 삼축으로 분화함을 보여준다. [[skill-curation-as-learning]]과의 병렬도 주목할 만하다 — 큐레이션의 대상이 스킬(축적물)에서 태스크(입력)로 이동한다.

## 🔗 관련 논문

- Strategically Diverse Sampling for Self-Training
- Shockingly Simple Self-retrospection Improves Agentic Models Without RL
- RetireOPD: Self-Retiring On-Policy Distillation for Agentic Reinforcement Learning
- Harness Learning Enables Generalizable Test-Time Adaptation

## 🏷️ 엔티티

- [[entities/gepa-curator.md|gepa-curator]]
- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/self-training-data-construction.md|self-training-data-construction]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]
- [[entities/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[entities/prompt-engineering.md|prompt-engineering]]
- [[entities/failure-as-causal-data.md|failure-as-causal-data]]
- [[entities/black-box-instrument-drift.md|black-box-instrument-drift]]

## 📐 개념

- [[concepts/learning-task-curation.md|learning-task-curation]]
- [[concepts/failure-source-attribution.md|failure-source-attribution]]
- [[concepts/strategic-diversity.md|strategic-diversity]]
- [[concepts/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[concepts/forgetting-as-accumulation-quality-management.md|forgetting-as-accumulation-quality-management]]

---
_LLM 분석으로 생성됨_
