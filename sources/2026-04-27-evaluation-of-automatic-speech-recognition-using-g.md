# Evaluation of Automatic Speech Recognition Using Generative Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-27
**링크**: http://arxiv.org/abs/2604.21928v1

## 💡 핵심 인사이트

WER가 의미에 무감각한 것은 메트릭의 결함이 아니라 평가 대상 자체의 오규정이며, 생성적 LLM을 ASR 평가 도구로 사용하는 것은 '정답과 얼마나 일치하는가'에서 '어떤 의미가 보존·상실되었는가'로 평가의 근본적 질문을 전환한다.

## 📖 분석

# Evaluation of Automatic Speech Recognition Using Generative Large Language Models

## 기존 Wiki와의 관계

본 논문은 [[entities/llm-as-judge|LLM-as-Judge]]의 적용 범위를 텍스트 생성 평가에서 음성 인식 평가로 확장하는 구체적 사례를 제공한다. 기존 Wiki에서 "LLM-as-Judge의 적용 범위가 ASR 후보 선택·의미 거리 계산 등 음성 도메인으로 확장됨"으로만 기술된 부분을 세 가지 방법론(쌍별 선택, 생성적 임베딩 기반 의미 거리, 정성적 오류 분류)으로 구체화한다.

## 핵심 기여

### WER의 구조적 한계 명식화
[[entities/word-error-rate|WER]]가 의미에 둔감하다는 비판을 넘어, 이것이 단순한 메트릭 결함이 아니라 **평가 대상 자체의 오규정**임을 보여준다. WER은 '음성이 텍스트로 얼마나 정확 변환되었는가'를 측정하지만, ASR의 실질적 목표인 '의미 보존 여부'와 구조적으로 정렬되지 않는다.

### 생성적 임베딩을 평가 도구로 전환
[[entities/generative-embedding-evaluation|생성적 임베딩 평가]] 엔티티에 실질적 내용을 제공한다: 디코더 기반 LLM의 생성적 임베딩을 의미 거리 계산에 활용하는 것이 기존 인코더 기반 임베딩과 어떻게 차별화되는지를 세 가지 접근법의 비교를 통해 구체화한다.

## 다른 논문과의 연결점

- [[sources/2026-04-26-mathduels-evaluating-llms-as-problem-posers-and-so.md|MathDuels]]와 공유하는 메타 주제: **평가자의 가정이 측정 결과를 어떻게 왜곡하는가**. MathDuels가 '정적 문제 집합'이라는 가정의 문제를 다룬다면, 본 논문은 '표면 형식 정합'이라는 가정의 문제를 다룬다.
- [[concepts/transitivity-violation|추이성 위반]]이 쌍별 후보 선택 방식에서 어떻게 현현할 수 있는지는 본 논문의 실험 설계가 직접 검증 가능한 구조를 제공한다.
- [[concepts/meaning-insensitive-metric|의미 무감각 메트릭]]의 대표 사례로 WER을 구체적으로 규정하여, 기존에 형식적이었던 이 개념에 도메인 특화적 실체를 부여한다.

## 🔗 관련 논문

- 2026-04-25-evaluation-of-automatic-speech-recognition-using-g.md
- 2026-04-26-evaluation-of-automatic-speech-recognition-using-g.md

## 🏷️ 엔티티

- [[entities/word-error-rate.md|word-error-rate]]
- [[entities/generative-embedding-evaluation.md|generative-embedding-evaluation]]
- [[entities/semantic-distance-metric.md|semantic-distance-metric]]
- [[entities/asr-evaluation.md|asr-evaluation]]
- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/hypothesis-selection-evaluation.md|hypothesis-selection-evaluation]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/audio-language-model.md|audio-language-model]]

## 📐 개념

- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/generative-embedding-as-metric.md|generative-embedding-as-metric]]
- [[concepts/hypothesis-selection-evaluation.md|hypothesis-selection-evaluation]]
- [[concepts/transitivity-violation.md|transitivity-violation]]
- [[concepts/decoder-based-llm-evaluation.md|decoder-based-llm-evaluation]]

---
_LLM 분석으로 생성됨_
