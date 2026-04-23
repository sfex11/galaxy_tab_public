# Can "AI" Be a Doctor? A Study of Empathy, Readability, and Alignment in Clinical LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-24
**링크**: http://arxiv.org/abs/2604.20791v1

## 💡 핵심 인사이트

LLM의 정렬 결함은 도메인에 따라 근본적으로 다른 양상으로 발현하며, 임상 환경에서는 팩트 오류가 아닌 감정 극성의 체계적 증폭으로 나타난다 — 이는 소통적 정렬이 안전성·유용성과 독립적인 제3의 정렬 차원임을 의미한다.

## 📖 분석

# Can "AI" Be a Doctor? 임상 LLM의 공감·가독성·정렬 연구

## 기존 Wiki와의 관계

이 논문은 [[entities/llm|LLM]]의 정렬 연구가 안전성·유용성에 집중된 현실에 대해 **소통적 정렬(communicative alignment)**이라는 새로운 축을 제시한다. 기존 [[concepts/llm-alignment|llm-alignment]]이 "해를 끼치지 않음"과 "유용함"을 다룬다면, 이 논문은 "인간 전문가의 감정적 보정 수준과 일치함"이라는 제3의 정렬 차원을 정량화한다.

특히 [[concepts/medical-ai|medical-ai]] 연구가 진단 정확도에 집중해온 것과 대비되며, [[concepts/clinical-reasoning|clinical-reasoning]]이 환자와의 소통 능력까지 포함해야 함을 실증한다.

## 핵심 발견

베이스라인 모델은 의사 대비 감정 극성을 체계적으로 증폭시킨다(Very Negative: 43.14–45.10% vs 의사). 도메인 특화 모델은 의미적 충실도는 개선하나 감정적 공명에서 여전히 의사와 괴리를 보인다. 이는 [[concepts/asymmetric-alignment-fragility|비대칭 정렬 취약성]]의 임상적 사례로 읽힌다 — 정렬이 "팩트"에서는 작동하지만 "감정"에서는 근본적으로 다른 거동을 보인다.

## 다른 논문과의 연결

- [[sources/2026-04-03-blinded-radiologist-and-llm-based-evaluation-of-ll.md|Blinded Radiologist Evaluation]]: 의학적 설명의 질 평가라는 공통 관심사를 공유하나, 이 논문은 감정·가독성 차원을 추가
- [[concepts/personalized-reward-model|personalized-reward-model]]: 개인화 보상 모델이 감정적 보정을 어떻게 학습할 수 있는지에 대한 방법론적 연결점

## 🔗 관련 논문

- 2026-04-03-blinded-radiologist-and-llm-based-evaluation-of-ll.md

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/medical-ai.md|medical-ai]]

## 📐 개념

- [[concepts/communicative-alignment.md|communicative-alignment]]
- [[concepts/affective-polarity-amplification.md|affective-polarity-amplification]]
- [[concepts/clinical-readability-evaluation.md|clinical-readability-evaluation]]

---
_LLM 분석으로 생성됨_
