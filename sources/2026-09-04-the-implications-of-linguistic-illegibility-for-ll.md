# The Implications of Linguistic Illegibility for LLM Security

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02852v1

## 💡 핵심 인사이트

LLM의 외부화된 언어 산출물과 기제적으로 추출한 언어 특징 모두 내부 연산의 신뢰할 수 없는 대리물이므로, 언어 표면에 의존하는 LLM 보안의 감시·인증 체계는 구조적 맹점을 갖는다.

## 📖 분석

## 핵심 개념: 언어적 판독불가능성 (Linguistic Illegibility)

이 논문은 LLM의 **외부화된 언어 출력과 기제적(mechanistic) 프로브로 추출된 언어 특징이 모두 내부 연산을 대표하지 못하는** 시나리오를 'linguistic illegibility'로 명명하고, 이것이 LLM 보안에 미치는 구조적 함의를 논한다.

## 기존 Wiki와의 관계

- [[risk-translation-loss-as-safety]]가 제기한 '안전한 출력 = 위험 정보의 번역 손실' 역설을 조작적 개념으로 일반화한다.
- [[hidden-state-risk-space]]의 은닉 상태 위험 가설에 이론적 뼈대를 제공한다.
- [[agent-execution-semantic-opacity]]의 불투명성을 에이전트-OS 경계에서 모델-언어 경계로 확장한다.

## 보안 함의

1. **표면 감시의 한계**: 프롬프트 모니터링·출력 필터링은 [[shadow-certification]]의 확장판이다.
2. **기제적 판독의 불충분성**: [[probe-cascade]], pre-decoding-refusal-detection 같은 활성화 판독 기법의 신뢰 전제가 흔들린다.
3. **잠재 채널 위험**: [[latent-communication-channel]]과 [[kv-cache-information-leakage]]가 시사하듯 언어에 실체화되지 않은 채널이 주요 공격면이 된다.
4. **인증 이중 하락**: [[will-source-inaccessibility]]를 넘어, 내부에 접근해도 언어 산출물의 왜곡된 대표를 피할 수 없다.

결론: 검증 대상이 언어 표면에서 연산 구조로 이동해야 하며, 이는 [[algorithm-system-translation-gap]]의 번역 손실 문제와 동형이다.

## 🔗 관련 논문

- Discovering a Shared Logical Subspace: Steering LLM Logical
- MoRFI: Monotonic Sparse Autoencoder Feature Identification
- From Syntax to Emotion: A Mechanistic Analysis of Emotion In
- LCGuard: Latent Communication Guard for Safe KV Sharing in M
- Crafting Reversible SFT Behaviors in Large Language Models

## 🏷️ 엔티티

- [[entities/ai-safety.md|ai-safety]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/agent-execution-semantic-opacity.md|agent-execution-semantic-opacity]]
- [[entities/hidden-state-risk-space.md|hidden-state-risk-space]]
- [[entities/risk-translation-loss-as-safety.md|risk-translation-loss-as-safety]]
- [[entities/latent-communication-channel.md|latent-communication-channel]]
- [[entities/kv-cache-information-leakage.md|kv-cache-information-leakage]]
- [[entities/shadow-certification.md|shadow-certification]]
- [[entities/alignment-base-opacity.md|alignment-base-opacity]]
- [[entities/locational-opacity-of-risk.md|locational-opacity-of-risk]]
- [[entities/llm-alignment.md|llm-alignment]]

## 📐 개념

- [[concepts/linguistic-illegibility.md|linguistic-illegibility]]
- [[concepts/risk-translation-loss-as-safety.md|risk-translation-loss-as-safety]]
- [[concepts/hidden-state-risk-space.md|hidden-state-risk-space]]
- [[concepts/agent-execution-semantic-opacity.md|agent-execution-semantic-opacity]]
- [[concepts/shadow-certification.md|shadow-certification]]
- [[concepts/mechanistic-probe-unreliability.md|mechanistic-probe-unreliability]]

---
_LLM 분석으로 생성됨_
