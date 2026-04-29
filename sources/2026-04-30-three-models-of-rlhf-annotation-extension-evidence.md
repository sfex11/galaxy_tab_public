# Three Models of RLHF Annotation: Extension, Evidence, and Authority

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25895v1

## 💡 핵심 인사이트

RLHF는 '인간 피드백'이라는 단일 레이블 아래 세 가지 근본적으로 다른 규범적 역할(연장·증거·권위)을 혼용하고 있으며, 이 혼용이 정렬의 정당성과 책임 귀속에 대한 체계적 모호성을 초래한다.

## 📖 분석

# Three Models of RLHF Annotation: Extension, Evidence, and Authority

## 핵심 주제
RLHF에서 인간 주석자의 판단이 수행하는 **규범적 역할(normative role)**을 세 가지 모델로 분류하여, 현재 RLHF 실무가 이 역할을 명시하지 않은 채 혼용하고 있음을 지적한다.

## 세 가지 모델
1. **Extension(연장)**: 주석자가 시스템 설계자 자신의 판단을 연장하는 도구
2. **Evidence(증거)**: 주석자가 독립적 사실에 대한 증거를 제공하는 정보원
3. **Authority(권위)**: 주석자가 독립적인 규범적 권위로서 시스템 행동의 근거가 됨

## Wiki와의 관계
기존 [[entities/llm-alignment|llm-alignment]] 엔티티는 RLHF를 '정렬 기법'으로 분류하지만, **정렬이 무엇에 대한 정렬인지**의 규범적 기초가 비어 있다. 본 논문은 이 빈칸을 세 가지 모델로 구조화하여, [[concepts/pluralistic-alignment|pluralistic-alignment]] 논의가 암묵적으로 전제하는 '권위 모델'의 문제점(누구의 권위인가?)을 [[entities/principal-identification-problem|principal-identification-problem]]과 직접 연결한다. 또한 [[concepts/evaluator-assumption|평가자의 가정]]이 벤치마크에만 국한된 것이 아니라 RLHF 주석 과정 자체에도 존재함을 보여준다.

## 연결점
- [[concepts/structural-value-alignment|structural-value-alignment]]: 세 모델은 구조적 정렬이 '구조적'인 이유를 규범적 기초에서 설명 가능하게 함
- [[concepts/safety-diversity-tradeoff|안전-다양성 트레이드오프]]: Extension 모델은 설계자의 판단을 연장하는 것이므로 본질적으로 다양성을 축소할 구조적 경향이 있음

## 🔗 관련 논문

- relative principals pluralistic alignment and the structural value a
- machine behavior in relational moral dilemmas moral rightne
- personalized rewardbench evaluating reward models with huma

## 🏷️ 엔티티

- [[entities/llm-alignment.md|llm-alignment]]
- [[entities/principal-identification-problem.md|principal-identification-problem]]

## 📐 개념

- [[concepts/annotator-normative-role.md|annotator-normative-role]]
- [[concepts/extension-model-of-annotation.md|extension-model-of-annotation]]
- [[concepts/evidence-model-of-annotation.md|evidence-model-of-annotation]]
- [[concepts/authority-model-of-annotation.md|authority-model-of-annotation]]
- [[concepts/normative-foundations-of-alignment.md|normative-foundations-of-alignment]]

---
_LLM 분석으로 생성됨_
