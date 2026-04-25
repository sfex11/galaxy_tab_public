# Machine Behavior in Relational Moral Dilemmas: Moral Rightness, Predicted Human Behavior, and Model Decisions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21871v1

## 💡 핵심 인사이트

LLM의 도덕 판단에서 규범적 정당성(무엇이 옳은가)과 기술적 예측(사람들이 무엇을 할 것인가) 사이의 체계적 괴리는, 도덕적 정렬이 보편적 규칙의 내면화가 아니라 관계적 맥락에 따른 규범 추론의 능력으로 재정의되어야 함을 보여준다.

## 📖 분석

# Machine Behavior in Relational Moral Dilemmas (2026-04-26)

## 핵심 질문
LLM이 인간의 도덕 판단을 모델링할 때 대인관계라는 사회적 맥락을 정확히 인코딩하는가?

## 연구 설계
Whistleblower's Dilemma를 실험 패러다임으로 사용하여 **범죄 심각성(crime severity)**과 **관계적 밀접성(relational closeness)** 두 차원을 변화시키며 세 가지 관점을 평가: (1) 도덕적 정당성(규범적), (2) 인간 행동 예측(기술적), (3) 모델 자체의 결정.

## 기존 Wiki와의 관계

### [[entities/llm-alignment|LLM 정렬]]으로의 확장
기존 정렬 연구가 단일 보편적 가치 기준에 대한 준수를 다뤘다면, 본 논문은 **관계적 맥락에 따라 도덕 정답이 변하는 상황**에서 정렬이 어떻게 작동하는지를 문제화한다. [[entities/relative-principals-pluralistic-alignment|Relative Principals]] 논문이 '누구의 원리인가'를 구조적으로 분석했다면, 본 논문은 그 원리의 내용(관계적 도덕)을 실증적으로 탐구하는 상보적 연구다.

### [[entities/ai-safety|AI 안전성]]과의 연결
도덕 판단의 관계적 변동성은 [[concepts/evaluator-assumption|평가자의 가정]] 문제와 직결된다. 정적 벤치마크에서 '올바른' 도덕적 응답을 정의하는 것은 관계적 맥락을 무시하는 것과 같으며, SafetyALFRED가 지적한 disembodied 평가의 한계를 도덕 영역에서 재현한다.

### [[entities/benchmark|벤치마크]] 패러다임에 대한 시사
세 가지 관점(규범/기술/결정)을 분리하여 평가하는 방법론은 [[entities/robogrid|RoboGrid]]가 구문·행동·의미를 분리한 것과 유사한 패턴 — 단일 점수가 아닌 평가 차원의 분해가 평가의 타당성을 높인다.

## 새로운 인사이트
LLM의 도덕 판단이 인간의 관계적 도덕 직관을 단순히 '평균내는' 것이 아니라, 규범적 판단과 기술적 예측 사이에 체계적 괴리를 보일 가능성을 제시한다. 이는 도덕적 정렬이 '무엇이 옳은가'와 '사람들이 무엇을 할 것인가'를 구분하지 못하면 실제 배포에서 사회적 신뢰를 훼손할 수 있음을 시사한다.

## 🔗 관련 논문

- 2026 04 24 relative principals pluralistic alignment and the
- 2026 04 23 safetyalfred evaluating safety conscious planning
- 2026 04 24 diagnosing cfg interpretation in llms
- 2026 04 24 can ai be a doctor a study of empathy readability

## 🏷️ 엔티티

- [[entities/relational-moral-dilemma.md|relational-moral-dilemma]]
- [[entities/machine-behavior.md|machine-behavior]]
- [[entities/llm-alignment.md|llm-alignment]]

## 📐 개념

- [[concepts/relational-moral-dilemma.md|relational-moral-dilemma]]
- [[concepts/prescriptive-vs-descriptive-moral-reasoning.md|prescriptive-vs-descriptive-moral-reasoning]]
- [[concepts/relational-closeness-modulation.md|relational-closeness-modulation]]
- [[concepts/whistleblower-dilemma.md|whistleblower-dilemma]]

---
_LLM 분석으로 생성됨_
