# Earlybird: Predictive Streaming Speech Recognition in 29M Parameters

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14421v1

## 💡 핵심 인사이트

음성 에이전트의 반응 지연 병목은 생성 계층이 아니라 지각 계층(단어 완료 대기)에 있으며, 무작위 절단 훈련으로 부분 음향 증거에서 선제 커밋하도록 만든 초소형 인식기가 이 병목을 제거한다.

## 📖 분석

## 핵심 기여

Earlybird는 29M 파라미터(4bit에서 16.8MB)의 초소형 스트리밍 음성 인식기로, '단어가 끝날 때까지 기다렸다가 출력'이라는 스트리밍 ASR의 암묵적 규약을 폐기한다. 무작위 지점에서 잘린 오디오(단어 중간 포함)로 훈련하여, 해당 시점까지 완료 예정인 모든 단어를 전체 형태로 예측 출력하고 진행 중인 단어에 대한 추측(guess)까지 덧붙인다. 이로써 90-400ms의 완료 대기 지연을 제거하고 음성 에이전트가 검색·답변 계획을 더 일찍 시작하게 한다.

## Wiki에서의 위치

지연 예산 논의의 상류 확장이다. RetroThinker가 발화 후 회고로 출력 계층의 지연 제약을 다뤘다면, 본 논문은 그 상류인 인식 지연을 공략하여 [[latency-constrained-reasoning]]의 예산에서 지각 단계를 축소한다. 인식 결과의 조기 출력은 [[in-turn-adaptation]]과 풀듀플렉스 음성 에이전트([[nemotronlabs-voicechat]])가 요구하는 실시간 입력 흡수의 전제조건을 지각 계층에서 공급하는 사례다.

29M 파라미터 선택은 [[lightweight-executor]] 원리(Jev-Mobile의 저빈도 계획-고빈도 경량 실행)의 지각 계층 실현이며, 늦은 출력 자체가 일시적 사건 대응을 놓치게 한다는 [[transient-event-miss-failure]]의 지각 계층 버전을 직접 겨냥한다. 방법론적으로 완료 전 선제 커밋은 [[speculative-decoding]]의 초안-검증 구조와 달리 검증자 없는 단발 예측이라는 대안 극점을 제공하며, 부분 증거에서 완전한 결정을 산출한다는 점에서 [[access-planning-gap]]의 지각 도메인 대응이다.

## 🔗 관련 논문

- Jev-Mobile: Jev as an Executor for Mobile GUI Agents (2026-09-26)
- RetroThinker: Enabling Retrospective Thinking in Speech LLMs (2026-09-12)
- NemotronLabs VoiceChat: An Open Full-duplex Speech-to-Speech Model wit (2026-09-22)

## 🏷️ 엔티티

- [[entities/earlybird.md|earlybird]]

## 📐 개념

- [[concepts/anticipatory-word-emission.md|anticipatory-word-emission]]
- [[concepts/truncation-scheduled-training.md|truncation-scheduled-training]]
- [[concepts/latency-constrained-reasoning.md|latency-constrained-reasoning]]
- [[concepts/in-turn-adaptation.md|in-turn-adaptation]]
- [[concepts/lightweight-executor.md|lightweight-executor]]
- [[concepts/transient-event-miss-failure.md|transient-event-miss-failure]]
- [[concepts/access-planning-gap.md|access-planning-gap]]
- [[concepts/speculative-decoding.md|speculative-decoding]]
- [[concepts/streaming-adaptive-inference.md|streaming-adaptive-inference]]

---
_LLM 분석으로 생성됨_
