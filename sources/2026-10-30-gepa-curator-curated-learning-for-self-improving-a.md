# GEPA-Curator: Curated Learning for Self Improving Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37651v1

## 💡 핵심 인사이트

실패가 학습 데이터가 되려면 그 원인이 에이전트의 학습 가능 요인(프롬프트)에 귀속되어야 하며, 하네스 한계·실행 확률성·judge 잡음에서 온 실패를 수용하면 개선이 아니라 퇴행이 학습된다.

## 📖 분석

# GEPA-Curator: Curated Learning for Self Improving Agents

## 핵심 주장

GEPA 계열 반사적(reflective) 프롬프트 최적화기는 실패 롤아웃에서 학습하지만, 에이전틱 실패의 원인은 이질적이다 — 프롬프트 약점(학습 가능), 하네스 한계, 확률적 실행, judge 잡음(학습 불가). 모든 실패를 무차별 수용하면 최적화기가 존재하지 않는 프롬프트 결함을 '수정'하려 시도하여 오히려 순진한 행동을 학습한다. GEPA-Curator는 학습 루프 상류에 태스크 큐레이션 단계를 도입해, 실패가 학습 가치를 갖는 태스크만 최적화기에 공급한다.

## Wiki 통합 관점

- [[learning-task-curation]] — 학습 데이터 구성의 축이 '추출 방식'에서 '태스크 선택'으로 상류 이동
- [[failure-source-attribution]] — 실패의 원인 귀속 가능성이 데이터 채택 판정 기준으로 격상
- [[training-process-gaming]] — Exploration Hacking(모델 측 훈련 저항)과 대비되는 데이터 측 방어
- [[skill-curation-as-learning]] — 큐레이션 대상을 스킬(산출물)에서 태스크(입력)로 확장
- [[self-improving-agent]] — 자기 개선의 성립 조건으로 실패 학습 가능성 판별 명시

## 연결점

- [[evaluation-regimes-information-bottleneck]]: 극단적 패스율 태스크는 신호 엔트로피가 붕괴하므로, 태스크 선별은 학습 신호의 정보량 확보 문제이기도 하다
- [[judge-instrument-reliability]]: judge 잡음이 프롬프트 결함으로 오귀인되면 큐레이션 판정 자체가 오염 — 측정 신뢰성이 큐레이션의 입력 변수가 된다
- EarlyEval과 상보: 평가 비용 절감(조기 예측)과 학습 신호 품질 보장(태스크 선별)의 두 축

## 핵심 인사이트

실패의 학습 가치는 그 원인이 에이전트의 학습 가능 요인에 귀속되는가에 달려 있으며, 귀속 불가능한 실패의 데이터 수용은 개선이 아니라 퇴행을 낳는다.

## 🔗 관련 논문

- SkillOS: Learning Skill Curation for Self-Evolving Agents
- Exploration Hacking: Can LLMs Learn to Resist RL Training?
- EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction

## 🏷️ 엔티티

- [[entities/gepa-curator.md|gepa-curator]]
- [[entities/self-improving-agent.md|self-improving-agent]]
- [[entities/training-process-gaming.md|training-process-gaming]]
- [[entities/skill-curation-as-learning.md|skill-curation-as-learning]]
- [[entities/judge-instrument-reliability.md|judge-instrument-reliability]]

## 📐 개념

- [[concepts/learning-task-curation.md|learning-task-curation]]
- [[concepts/failure-source-attribution.md|failure-source-attribution]]
- [[concepts/failure-as-causal-data.md|failure-as-causal-data]]
- [[concepts/self-training-data-construction.md|self-training-data-construction]]
- [[concepts/evaluation-regimes-information-bottleneck.md|evaluation-regimes-information-bottleneck]]

---
_LLM 분석으로 생성됨_
