# Playing log(N)-Questions over Wikipedia Abstracts: Communication Efficiency Between Paired Frontier Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19113v1

## 💡 핵심 인사이트

동일 모델 쌍의 정보 비대칭 통신 게임은 이종성 없이도 자연어 채널에서 발생하는 번역 손실을 격리·정량화하며, 정확히 log₂(N) 질문 예산이 정보론적 비트 상한 대비 통신 효율의 절대 측정을 가능하게 한다.

## 📖 분석

# log(N)-Questions 게임: 쌍대 프론티어 모델의 통신 효율 (2026-09-18)

질문자가 N개 위키피디아 리드 단락 중 비밀 타깃을 정확히 log₂(N)개의 yes/no 질문으로 식별하고, 응답자는 타깃과 질문만 보고 한 단어로 답하는 2인 게임. 동일 제공자의 모델 쌍이 양역을 수행하여, 정보 비대칭 하에서 모델이 스스로와 얼마나 잘 통신하는지를 측정한다.

## Wiki와의 관계

[[inter-agent-translation-gap]]에 최초의 통제된 측정 기기를 제공한다 — 이종 모델 간 번역 손실 논의와 달리 동일 모델 쌍의 자기 통신을 격리하여, 번역 간극이 이종성 없이도 자연어 채널에서 발생함을 보여준다. 동일 가중치 양역은 [[latent-communication-homogeneity-dependency]]의 극단 구성으로, 완전 동질성이 통신 성공을 보장하지 않음을 시사한다.

정확히 log₂(N) 질문 예산은 [[information-theoretic-capacity]]의 비트 상한을 평가 조건으로 연산화한다 — 균등 사전의 엔트로피를 정확히 소진하도록 강제하여 질문당 실현 정보량을 1비트 천장 대비 정량화한다. 동일 원천 간 합의가 올바름을 담보하지 못한다는 [[consistency-correctness-divergence]] 비판의 역발상으로, 여기서는 동일성을 진단 조건으로 전용해 실패를 내부 표현-통신 정렬 결함으로 국소화한다. 질문자의 가설 공간 분할과 응답자의 단어 디코딩은 [[theory-of-mind]]의 최소 실험이며, N=4→1024 스케일링과 한 단어 채널 설계는 [[llm-benchmark]]에 정보론적 분모를 갖는 새 평가 패러다임을 추가한다.

## 🔗 관련 논문

- Mind2Dialogue: Training Human-Aware Language Models by Simulating User (2026-09-16)
- Copying explains the collective behavior of AI agents in the (2026-09-10)

## 🏷️ 엔티티

- [[entities/inter-agent-translation-gap.md|inter-agent-translation-gap]]
- [[entities/information-theoretic-capacity.md|information-theoretic-capacity]]
- [[entities/self-communication-fidelity.md|self-communication-fidelity]]
- [[entities/agent-coordination.md|agent-coordination]]
- [[entities/consistency-correctness-divergence.md|consistency-correctness-divergence]]
- [[entities/latent-communication-homogeneity-dependency.md|latent-communication-homogeneity-dependency]]
- [[entities/theory-of-mind.md|theory-of-mind]]
- [[entities/llm-benchmark.md|llm-benchmark]]

## 📐 개념

- [[concepts/self-communication-fidelity.md|self-communication-fidelity]]
- [[concepts/exact-entropy-question-budget.md|exact-entropy-question-budget]]
- [[concepts/same-provider-pairing.md|same-provider-pairing]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-18-flag-game-a-toy-model-for-mechanistic-swarm-interp]]: 통제된 게임 프로토콜(log₂(N) 질문 예산, 숨겨진 국기)로 정보 비대칭 하의 자연어 통신 손실과 집단 신념 역학을 격리·정량화한다는 방법론을 공유한다.
