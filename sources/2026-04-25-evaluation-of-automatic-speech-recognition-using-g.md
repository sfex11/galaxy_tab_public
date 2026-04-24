# Evaluation of Automatic Speech Recognition Using Generative Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-25
**링크**: http://arxiv.org/abs/2604.21928v1

## 💡 핵심 인사이트

WER의 의미 무감각성은 평가 메트릭의 기술적 결함이 아니라, '정확한 전사'와 '의미 보존' 사이의 인식론적 단절을 반영하는 구조적 문제이며, 생성적 LLM을 평가자로 사용하는 것은 이 단절을 메우는 시도이지만 LLM-as-Judge의 이미 알려진 일관성 문제를 동시에 상속한다.

## 📖 분석

# ASR 평가에서 생성적 LLM의 적용 가능성

기존 자동 음성 인식(ASR) 평가는 **Word Error Rate (WER)**에 의존해왔으나, WER은 의미 보존에 무감각하다는 근본적 한계가 있다. 본 논문은 디코더 기반 생성적 LLM을 ASR 평가자로 활용하는 세 가지 접근법을 체계적으로 검증한다: (1) 두 후보 가설 중 최선 선택, (2) 생성적 임베딩을 활용한 의미 거리 계산, (3) 정성적 분류.

## 기존 Wiki와의 관계

이 논문은 Wiki에 이미 축적된 **LLM-as-Judge** 패턴을 음성 인식 도메인으로 확장한다. 기존 Wiki가 지적한 LLM-as-Judge의 구조적 문제—**추이성 위반**, **인스턴스 수준 일관성 감사**의 필요성—은 ASR 평가에서도 동일하게 적용된다. WER의 의미 무감각성 문제는 **인식론적 충실도** 개념과 직결된다: 우리가 '정확한 전사'를 측정한다고 믿지만, 실제로 관심 있는 것은 '의미 보존'이며, 두 지표 사이의 간극이 바로 인식론적 단절의 한 형태다.

또한 **LALM**(오디오 언어 모델) 연구 축에서 밝혀진 "LLM 백본의 청각 도메인 지식이 LALM 성능 상한을 결정한다"는 발견과 연결된다. ASR 평가에 LLM을 사용한다는 것은 LLM이 내재한 음성-의미 매핑 지식을 평가 도구로 전용하는 것이며, 이 지식의 질이 평가 신뢰성의 상한선이 된다.

## 새로운 관점

WER → 의미 기반 평가로의 전환은 단순한 메트릭 교체가 아니다. 이는 **평가의 인식론적 기준 자체를 재정의**하는 시도로, 벤치마크 연구가 '무엇을 측정하는가'보다 '어떻게 측정하는가'에 집중해온 한계를 드러낸다.

## 🏷️ 엔티티

- [[entities/llm.md|llm]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/lalm.md|lalm]]
- [[entities/audio-language-model.md|audio-language-model]]

## 📐 개념

- [[concepts/word-error-rate.md|word-error-rate]]
- [[concepts/asr-evaluation.md|asr-evaluation]]
- [[concepts/semantic-distance-metric.md|semantic-distance-metric]]
- [[concepts/generative-embedding-evaluation.md|generative-embedding-evaluation]]

---
_LLM 분석으로 생성됨_
