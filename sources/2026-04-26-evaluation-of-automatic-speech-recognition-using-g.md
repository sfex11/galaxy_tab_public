# Evaluation of Automatic Speech Recognition Using Generative Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-26
**링크**: http://arxiv.org/abs/2604.21928v1

## 💡 핵심 인사이트

WER의 의미 무감각성은 평가 메트릭 자체가 만들어내는 형식 인공물이며, 생성형 LLM의 의미 이해 능력을 평가 도구로 직접 활용하는 것이 ASR 평가의 구조적 한계를 해결하는 실증적 경로다.

## 📖 분석

# Evaluation of Automatic Speech Recognition Using Generative Large Language Models (2026-04-26)

## 핵심 주장
ASR 평가의 표준인 WER(Word Error Rate)이 의미 보존에 무감각하다는 근본적 한계를 지적하고, 디코더 기반 생성형 LLM을 세 가지 방식으로 ASR 평가에 활용 가능함을 실증한다: (1) 두 후보 간 최선 가설 선택, (2) 생성형 임베딩 기반 의미 거리 계산, (3) 정성적 분류.

## 기존 Wiki와의 관계

### LLM-as-Judge의 도메인 확장
기존 `llm-as-judge` 개념이 텍스트 생성 평가에 집중된 반면, 본 논문은 이를 음성 인식 평가라는 새로운 도메인으로 확장한다. 특히 기존 Wiki에서 지적된 **추이성 위반(transitivity violation)** 문제가 ASR 평가에서도 잠재적 위협이 됨을 시사한다 — 두 후보 간 선택 평가(방식 1)를 사용할 경우 이 문제가 직접적으로 관련된다.

### 의미 무감각 메트릭에 대한 구조적 비판
WER의 한계는 Wiki의 여러 논문들이 제기한 **평가자의 가정(evaluator-assumption)** 문제의 구체적 사례다. 벤치마크 설계자가 '정확한 전사=좋은 인식'이라는 암묵적 가정을 WER에 내재시켜, 실제 사용자 경험(의미 보존)과 측정값 사이에 구조적 격차를 생성한다. 이는 `safetyalfred`가 지적한 **평가 형식 인공물(evaluation-format-artifact)**과 동일한 패턴이다.

### 생성형 임베딩의 평가 도구화
방식 2(생성형 임베딩 기반 의미 거리)는 임베딩이 표현(representation) 학습 도구를 넘어 평가 메트릭 자체로 기능함을 보여준다. 기존 `semantic-distance-metric` 개념의 실증적 근거를 제공하며, `text-embedding`의 '비합리적 효과성'이 평가 영역으로도 확장됨을 시사한다.

## 다른 논문과의 연결점
- **MathDuels**: 고정 문제 집합의 천장 성능 문제와 유사하게, WER이라는 고정 메트릭도 ASR 시스템 발전에 따른 의미적 미세 차이를 포착하지 못하는 천장에 도달했을 가능성이 있다.
- **SWE-chat**: 실제 사용 환경에서의 평가 필요성과 맞닿아 있으며, WER은 실제 사용자가 인식하는 '의미적 충실도'를 대변하지 못한다는 점에서 `task-reality-divergence`의 음성 도메인 인스턴스다.

## 🔗 관련 논문

- 2026-04-25-mathduels-evaluating-llms-as-problem-posers-and-so.md
- 2026-04-24-swe-chat-coding-agent-interactions-from-real-users.md
- 2026-04-23-safetyalfred-evaluating-safety-conscious-planning-.md

## 🏷️ 엔티티

- [[entities/llm-as-judge.md|llm-as-judge]]
- [[entities/semantic-distance-metric.md|semantic-distance-metric]]
- [[entities/word-error-rate.md|word-error-rate]]
- [[entities/audio-language-model.md|audio-language-model]]
- [[entities/llm-benchmark.md|llm-benchmark]]
- [[entities/generative-embedding-evaluation.md|generative-embedding-evaluation]]
- [[entities/asr-evaluation.md|asr-evaluation]]

## 📐 개념

- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/hypothesis-selection-evaluation.md|hypothesis-selection-evaluation]]
- [[concepts/generative-embedding-as-metric.md|generative-embedding-as-metric]]

---
_LLM 분석으로 생성됨_
