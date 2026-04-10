# TiCo: Time-Controllable Training for Spoken Dialogue Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22267v1

## 💡 핵심 인사이트

음성 대화 모델에 시간 인식 능력을 부여하는 경량 포스트 트레이닝 방법으로, 실제 음성 에이전트의 응답 길이 제어라는 실용적 문제를 해결한다.

## 📖 분석

## TiCo: Time-Controllable Training for Spoken Dialogue Models

**arXiv**: http://arxiv.org/abs/2603.22267v1
**날짜**: 2026-03-25

TiCo는 음성 대화 모델(Spoken Dialogue Models, SDMs)이 시간 제약 지시를 따르고 제어 가능한 길이의 응답을 생성할 수 있도록 하는 간단한 포스트 트레이닝 방법이다. 음성 비서나 대화형 에이전트 같은 실제 음성 언어 시스템에서 응답 길이를 제어하는 것은 상호작용 품질 향상에 핵심적이지만, 기존 모델들은 시간 인식(time awareness) 능력이 부족하여 이러한 지시를 따르는 데 어려움을 겪는다.

### 핵심 기여

- **시간 제어 가능한 생성**: 기존 SDM에 포스트 트레이닝을 적용하여 "30초 이내로 답변해줘"와 같은 시간 제약 지시를 따를 수 있게 함
- **간단한 포스트 트레이닝 접근**: 복잡한 아키텍처 변경 없이 기존 모델 위에 적용 가능한 경량 방법론
- **실용적 가치**: 음성 비서, 대화형 에이전트 등 실시간 음성 시스템에서의 사용자 경험 개선에 직결

### Wiki 연결점

이 연구는 [[post-training]] 개념과 직접적으로 관련되며, 기존 모델의 능력을 확장하기 위해 추가 학습을 적용하는 접근법을 공유한다. 또한 [[audio-language-model]] 및 [[audio-question-answering]] 분야의 확장으로, 음성 모델의 제어 가능성이라는 새로운 축을 제시한다. LLM Agent 엔티티와도 연결되는데, 음성 에이전트가 실제 환경에서 시간 제약 하에 동작해야 하는 요구사항을 다루기 때문이다.

## 🔗 관련 논문

- 2026 04 08 how ai aggregation affects knowledge
- 2026 03 21 how auditory knowledge in llm backbones shapes aud

## 📐 개념

- [[concepts/post-training.md|post-training]]
- [[concepts/audio-language-model.md|audio-language-model]]
- [[concepts/audio-question-answering.md|audio-question-answering]]

---
_LLM 분석으로 재생성됨_
