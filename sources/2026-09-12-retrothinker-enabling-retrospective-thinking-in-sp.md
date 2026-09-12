# RetroThinker: Enabling Retrospective Thinking in Speech LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-12
**링크**: http://arxiv.org/abs/2609.11864v1

## 💡 핵심 인사이트

사고를 응답 이전에서 응답 이후로 재배치하는 회고적 추론은, 지연 민감한 실시간 음성 상호작용에서 추론 깊이와 응답 지연의 트레이드오프를 연산량 절감이 아닌 출력 순서의 재설계라는 제3의 해법으로 전환한다.

## 📖 분석

# RetroThinker: Enabling Retrospective Thinking in Speech LLMs

**arXiv**: 2609.11864 (2026-09-12)

## 핵심 주장

SpeechLLM은 ASR 캐스케이드를 우회해 지연을 줄이고 부가언어적(paralinguistic) 정보를 보존하지만, 복잡한 추론에서 텍스트 전용 LLM에 뒤처지며 실시간 음성 상호작용의 엄격한 지연 제약과 충돌한다. RetroThinker는 사고(thinking)를 응답 '이전'이 아닌 '이후'에 배치하는 회고적 추론(retrospective thinking) 패러다임을 제안한다 — 빠른 초기 응답을 먼저 내보낸 뒤, 사후 사고로 이를 정제한다.

## 기존 Wiki 논의와의 관계

[[adaptive-inference]]의 적응 축에 시간 배치 차원('언제 계산하는가')을 추가한다. 기존 논의가 예산 축(얼마나 계산할까)과 궤적 축(어떤 방향으로)을 다뤘다면, 본 논문은 추론 연산의 출력 대비 위치 자체를 독립 설계 변수로 격상시킨다. 이는 [[inference-budget-progressive-investment]]의 초기 응답 후 점진 투입 원리를 음성 도메인에서 실현한 사례이며, [[streaming-adaptive-inference]]의 실시간 제약 하 깊은 추론 유지 과제에 대한 구체적 해법이다.

[[thought-action-topology]] 관점에서 [사고→행동]의 선형 순서를 [행동→사고→정제]로 역전시켜 CoT의 지연 비용을 상호작용 흐름 속에 은닉하는 위상 변형 사례다. 음성 모달의 추론 격차 진단은 [[slm-reasoning-gap]]의 모달리티 확장으로 읽히며, ASR 캐스케이드 대비 부가언어 보존 우위는 [[audio-language-model]]의 모달리티 정보 손실 논의와 직결된다.

## 🔗 관련 논문

- Evaluation of Automatic Speech Recognition Using Generative Large Language Models

## 🏷️ 엔티티

- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/audio-language-model.md|audio-language-model]]
- [[entities/streaming-adaptive-inference.md|streaming-adaptive-inference]]
- [[entities/inference-budget-progressive-investment.md|inference-budget-progressive-investment]]
- [[entities/thought-action-topology.md|thought-action-topology]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/retrospective-thinking.md|retrospective-thinking]]
- [[entities/speech-llm.md|speech-llm]]

## 📐 개념

- [[concepts/retrospective-thinking.md|retrospective-thinking]]
- [[concepts/speech-llm.md|speech-llm]]
- [[concepts/latency-constrained-reasoning.md|latency-constrained-reasoning]]

---
_LLM 분석으로 생성됨_
