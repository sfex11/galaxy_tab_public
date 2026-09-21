# NemotronLabs VoiceChat: An Open Full-duplex Speech-to-Speech Model with Tool Calling Capabilities

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-22
**링크**: http://arxiv.org/abs/2609.21967v1

## 💡 핵심 인사이트

풀듀플렉스 음성 에이전트에서 발화와 도구 호출이 병렬 특화 출력 스트림으로 통합되어, 음성 모델이 '말하는 인터페이스'에서 '동시에 행동하는 에이전트'로 재정의된다.

## 📖 분석

## NemotronLabs VoiceChat: 풀듀플렉스 음성 에이전트의 아키텍처적 실현

NemotronLabs VoiceChat은 도구 호출 능력을 네이티브로 갖춘 오픈 풀듀플렉스 speech-to-speech 모델이다. 스트리밍 음성 인코더와 디코더 전용 LM 위에 에이전트 텍스트·구조화 함수 호출을 위한 병렬 특화 출력 스트림, 점진적 사용자 전사용 보조 RNN-T 브랜치, 스트리밍 TTS 디코더를 결합하여 듣기·전사·추론·도구 호출·발화를 단일 스트리밍 파이프라인에서 수행한다.

### speech-llm 연구 지형에서의 위치

speech-llm 연구가 추론 축([[retrospective-thinking]] 계열의 회고)과 언어 커버리지 축(Nuha-Speech)으로 분화되어 온 지형에 제3의 직교 축인 **행동 축(네이티브 도구 호출)**을 공급한다. 음성 모델이 말하는 인터페이스가 아니라 환경에 작용하는 에이전트로 기능하며, 범용성의 정의가 음성 입출력 품질에서 동시 다중 스트림 에이전시로 확장된다.

핵심 아키텍처 기여는 사고-행동 분리의 음성 도메인 재정의다. 발화와 도구 호출이 순차가 아닌 병렬 스트림에서 동시 생성되므로, 분리가 '순서 제약'에서 '채널 전문화'로 이동한다. 이는 [[utterance-stream-concurrency-control]]이 규정한 '동시 활성 가능한 스트림들의 집합'이라는 발화 모델을 프로토콜 수준에서 아키텍처 수준으로 구현한 사례다.

발화 중 지속 청취는 [[in-turn-adaptation]]의 구조적 전제를 충족하고, 이미 발화된 출력의 비가역성([[emitted-output-irreversibility]]) 하에서 도구 결과를 실시간 반영하는 새 문제를 연다. MP-Bench가 음성 에이전트의 다자 참여를 평가 대상으로 삼았다면, 본 모델은 그에 부합하는 참여자 후보를 제공한다.

## 🔗 관련 논문

- RetroThinker: Enabling Retrospective Thinking in Speech LLMs
- Nuha-Speech: Building General-Purpose Arabic Speech-LLMs
- Continue, Adapt, or Yield: In-Turn Adaptation to Overlapping Speech in Full-Duplex Agents
- MP-Bench: Evaluating Voice Agents as a Multiparty Conversation Participant

## 🏷️ 엔티티

- [[entities/nemotronlabs-voicechat.md|nemotronlabs-voicechat]]
- [[entities/speech-llm.md|speech-llm]]
- [[entities/thought-action-separation.md|thought-action-separation]]
- [[entities/utterance-stream-concurrency-control.md|utterance-stream-concurrency-control]]
- [[entities/nvidia.md|nvidia]]
- [[entities/latency-constrained-reasoning.md|latency-constrained-reasoning]]

## 📐 개념

- [[concepts/speech-native-tool-calling.md|speech-native-tool-calling]]
- [[concepts/parallel-output-streams.md|parallel-output-streams]]
- [[concepts/in-turn-adaptation.md|in-turn-adaptation]]
- [[concepts/emitted-output-irreversibility.md|emitted-output-irreversibility]]
- [[concepts/multiparty-floor-management.md|multiparty-floor-management]]

---
_LLM 분석으로 생성됨_
