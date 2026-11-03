# ACCT: Asymmetric Cross-LLM Context Transfer

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42116v1

## 💡 핵심 인사이트

이종 LLM 간 KV 캐시 전이가 서빙 계층에서 실현되면 잠재 통신의 동질성 의존 전제가 반증되고, 컨텍스트는 모델 경계를 넘는 이식 가능한 자원이 된다.

## 📖 분석

ACCT는 이기종 LLM 배포에서 동적 모델 호출 시 동일 컨텍스트를 새로 선택된 대상 모델이 매번 재처리하는 반복 비용 문제를, 소스 모델의 KV 캐시를 대상 모델로 비대칭 전이하는 서빙 기법으로 해결한다.

기존 Wiki의 [[latent-communication-homogeneity-dependency]]는 KV 캐시 공유의 효율 이점이 동질적 구성에 의존하며 이종 모델 간 잠재 공간 정렬 불가능성으로 적용 범위가 수축한다고 규정했다. 본 논문은 정확히 그 불가능 영역—이종 LLM 간 KV 전이—을 서빙 계층 해법으로 실현하여 동질성 의존 전제의 첫 구조적 반례를 제공한다. 이에 따라 [[kv-cache-optimization]]의 대상이 단일 모델 서빙 내부에서 모델 경계 간 이식 자산으로 확장되고, [[agent-native-serving]]에 '크로스 모델 캐시 이식성'이라는 새 프리미티브가 추가된다.

또한 [[adaptive-inference]]와 [[computation-unit-meta-selection]]의 동적 모델 선택이 재처리 비용에 의해 경제성이 제한되어 있었음을 드러내며, 캐시 전이가 이 선택의 자유도를 회복시킨다. [[memory-portability]]가 텍스트 수준의 손실 번역을 통한 메모리 생존을 다뤘다면 ACCT는 잠재 표현 수준의 컨텍스트 이식성을 열어 [[text-artifact-limitation]]의 반대 방향 경로를 제시한다. 반면 [[kv-cache-information-leakage]]가 지적한 잠재 채널이 제도화된 전이 경로가 되므로, 전이 지점이 새로운 감사·통제 대상이 됨을 시사한다. [[kv-streams]]가 agentic RL의 반복 프리필 병목을 제거했다면 ACCT는 배포 시 이종 모델 호출의 동일 병목을 제거하여, '같은 컨텍스트를 두 번 계산하지 않는다'는 원리가 훈련과 배포 양축으로 확장됨을 보여준다.

## 🔗 관련 논문

- KV-streams for Efficient Compaction in Agentic Reinforcement Learning
- Turning the TIDE: Cross-Architecture Distillation for Diffusion Large Language Models
- EAServe: Encode-Aware Disaggregated Serving for Multimodal Large Language Models

## 🏷️ 엔티티

- [[entities/cross-llm-kv-cache-transfer.md|cross-llm-kv-cache-transfer]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/agent-native-serving.md|agent-native-serving]]
- [[entities/kv-streams.md|kv-streams]]
- [[entities/adaptive-inference.md|adaptive-inference]]
- [[entities/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[entities/memory-portability.md|memory-portability]]
- [[entities/cross-architecture-distillation.md|cross-architecture-distillation]]

## 📐 개념

- [[concepts/cross-llm-kv-cache-transfer.md|cross-llm-kv-cache-transfer]]
- [[concepts/latent-communication-homogeneity-dependency.md|latent-communication-homogeneity-dependency]]
- [[concepts/latent-communication-channel.md|latent-communication-channel]]
- [[concepts/kv-cache-information-leakage.md|kv-cache-information-leakage]]
- [[concepts/text-artifact-limitation.md|text-artifact-limitation]]
- [[concepts/prefix-misalignment.md|prefix-misalignment]]
- [[concepts/adaptive-inference.md|adaptive-inference]]
- [[concepts/agent-native-serving.md|agent-native-serving]]

---
_LLM 분석으로 생성됨_
