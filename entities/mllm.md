# Mllm: 합성 분석

**카테고리**: AI/ML
**관련 논문**: 21편
**분석 갱신일**: 2026-04-14

## 정의

멀티모달 대형 언어 모델(Multimodal Large Language Model, MLLM)은 텍스트, 이미지, 비디오, 오디오 등 다양한 모달리티를 통합 처리하는 대형 언어 모델의 확장이다. VLM(Vision-Language Model)을 포함하는 상위 개념으로, 시각-언어 이해를 넘어 3D 공간 추론, 에이전틱 행동, 도메인 특화 진단 등으로 능력 범위를 확장하고 있다.

## 핵심 연구 축

### 1. 공간 추론과 3D 이해의 확장

MLLM 연구의 가장 두드러진 흐름은 2D 시각-언어 능력을 3D 공간으로 확장하는 것이다. **Loc3R-VLM**은 단안 비디오만으로 명시적 3D 위치 추정을 수행하고, **3DCity-LLM**은 이를 도시 규모로 스케일업하여 coarse-to-fine 인코딩으로 다중 해상도 장면 이해를 달성했다. **Generation Models Know Space**는 비디오 생성 모델의 암묵적 3D 프라이어를 활용하는 패러다임 전환을 제시하며, **UniDriveVLA**는 자율주행에서 2D 의미 추론과 3D 공간 인지의 트레이드오프를 통합 아키텍처로 해결했다. 이 연구들은 MLLM이 언어적 이해를 넘어 기하학적·물리적 세계 모델을 내재화하는 방향으로 진화하고 있음을 보여준다.

### 2. 에이전틱 MLLM과 메타인지

MLLM을 자율적 에이전트로 확장하려는 시도가 활발하다. **MARCUS**는 심장 진단에서 이질적 의료 모달리티를 통합 추론하는 에이전틱 VLM을, **UI-Voyager**는 실패 궤적의 credit assignment를 통한 자기진화를, **AMIGO**는 다중 이미지 갤러리에서 능동적 추론 전략을 평가한다. 특히 **Act Wisely**와 **Stop Wandering**은 메타인지(metacognition)라는 공통 키워드로 수렴한다. 전자는 도구 호출 필요성의 자율 판단을, 후자는 VLN에서 탐색 전략의 자기 모니터링을 다루며, 에이전트가 단순 행동 생성을 넘어 자기 조절 능력을 갖춰야 한다는 합의를 형성한다.

### 3. 추론 효율화: 토큰 축소 vs. 어텐션 희소화

장기 비디오 등 대량 시각 입력의 처리 비용을 줄이기 위한 두 가지 직교적 전략이 경쟁한다. **AdaptToken**은 엔트로피 기반 글로벌 토큰 선택과 적응적 조기 종료를, **VISOR**는 토큰 제거 대신 레이어별 시각-언어 상호작용의 동적 선택을 제안한다. **SpecEyes**는 speculative decoding을 에이전트 파이프라인 수준으로 확장하여 인식-추론-도구호출 루프를 병렬화한다. 이들은 "무엇을 버릴 것인가" vs. "어디서 계산할 것인가"라는 상이한 관점에서 효율화를 추구하며, 상호 보완적 적용이 가능하다.

### 4. 시각 표현과 학습의 신뢰성

**Steerable Visual Representations**는 ViT 특징을 텍스트 조건부로 조종하여 MLLM의 언어 중심성과 순수 ViT의 비유도성 사이를 메우는 새로운 패러다임을 제시한다. 한편 **Hallucination in RL Post-Training**은 RL 후훈련이 시각적 추론을 개선하는 듯 보이지만 실제로는 텍스트 패턴 기반 환각에 의존한 단축 학습일 수 있다는 경고를 던진다. **OpenVLThinkerV2**가 GRPO 기반 RL로 지각-추론 균형을 추구하고 **MMEmb-R1**이 CoT 추론의 선택적 적용을 제안하는 맥락에서, RL 후훈련의 실질적 효과에 대한 환각 연구의 경종은 이 분야 전체의 방법론적 재검토를 요구한다.

## 논문 간 관계: 일치, 긴장, 보완

| 관계 | 논문 쌍 | 내용 |
|------|---------|------|
| **보완** | NavTrust ↔ Stop Wandering | 전자는 강건성 벤치마크, 후자는 효율적 탐색 전략으로 VLN의 신뢰성과 효율을 양면에서 다룸 |
| **긴장** | OpenVLThinkerV2 ↔ Hallucination in RL | RL 후훈련의 멀티모달 추론 개선 vs. 환각 의존 단축학습 가능성 |
| **수렴** | Act Wisely ↔ Stop Wandering ↔ Chameleon | 메타인지·메모리 관리라는 상위 인지 능력이 에이전틱 MLLM의 핵심 병목 |
| **직교** | AdaptToken ↔ VISOR | 토큰 축소 vs. 어텐션 희소화라는 독립적 효율화 축 |

## 미래 방향

1. **3D 공간 추론의 일반화**: 실내→도시 규모 확장은 달성되었으나, 동적 환경에서의 실시간 3D 추론과 물리 시뮬레이션 통합이 다음 과제다.
2. **메타인지의 체계화**: 도구 사용, 탐색 전략, 메모리 관리에 걸친 자기 조절 능력을 통합하는 범용 메타인지 프레임워크가 필요하다.
3. **RL 후훈련의 검증 방법론**: 환각 의존 단축학습 문제가 밝혀진 만큼, 시각적 추론 능력의 진정성을 검증하는 표준화된 평가 프로토콜이 시급하다.
4. **효율화 기법의 통합**: 토큰 선택, 어텐션 희소화, 파이프라인 병렬화를 결합한 계층적 효율화 전략의 탐구가 기대된다.

## 전체 관련 논문 (21편)

- [[sources/2026-03-19-loc3r-vlm-language-based-localization-and-3d-reaso.md|Loc3R-VLM]] (2026-03-19) — 단안 비디오 기반 3D 위치 추정
- [[sources/2026-03-22-generation-models-know-space-unleashing-implicit-3.md|Generation Models Know Space]] (2026-03-22) — 생성 모델의 암묵적 3D 프라이어
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md|NavTrust]] (2026-03-23) — 체화 내비게이션 신뢰성 벤치마크
- [[sources/2026-03-25-marcus-an-agentic-multimodal-vision-language-model.md|MARCUS]] (2026-03-25) — 심장 진단 에이전틱 VLM
- [[sources/2026-03-26-3dcity-llm-empowering-multi-modality-large-languag.md|3DCity-LLM]] (2026-03-26) — 도시 규모 3D MLLM
- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md|SpecEyes]] (2026-03-26) — 에이전틱 MLLM 추측적 가속
- [[sources/2026-03-26-vision-on-request-enhanced-vllm-efficiency-with-sp.md|VISOR]] (2026-03-26) — 희소 시각-언어 상호작용
- [[sources/2026-03-27-chameleon-episodic-memory-for-long-horizon-robotic.md|Chameleon]] (2026-03-27) — 장기 로봇 조작 에피소딕 메모리
- [[sources/2026-03-27-ui-voyager-a-self-evolving-gui-agent-learning-via-.md|UI-Voyager]] (2026-03-27) — 실패 경험 기반 자기진화 GUI 에이전트
- [[sources/2026-03-31-adapttoken-entropy-based-adaptive-token-selection-.md|AdaptToken]] (2026-03-31) — 엔트로피 기반 적응적 토큰 선택
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md|AMIGO]] (2026-04-01) — 다중 이미지 에이전틱 그라운딩 벤치마크
- [[sources/2026-04-03-unidrivevla-unifying-understanding-perception-and-.md|UniDriveVLA]] (2026-04-03) — 자율주행 이해·인지·행동 통합
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md|Stop Wandering]] (2026-04-04) — 메타인지 기반 VLN 효율화
- [[sources/2026-04-05-steerable-visual-representations.md|Steerable Visual Representations]] (2026-04-05) — 텍스트 조건부 시각 표현 조종
- [[sources/2026-04-07-understanding-the-role-of-hallucination-in-reinfor.md|Hallucination in RL Post-Training]] (2026-04-07) — RL 후훈련 환각 분석
- [[sources/2026-04-09-mmemb-r1-reasoning-enhanced-multimodal-embedding-w.md|MMEmb-R1]] (2026-04-09) — 추론 강화 멀티모달 임베딩
- [[sources/2026-04-11-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|OpenVLThinkerV2]] (2026-04-11) — 범용 멀티모달 추론 모델
- [[sources/2026-04-12-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|Act Wisely]] (2026-04-12) — 메타인지적 도구 사용
- [[sources/2026-04-12-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|OpenVLThinkerV2]] (2026-04-12) — 범용 멀티모달 추론 모델 (갱신)
- [[sources/2026-04-13-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|Act Wisely]] (2026-04-13) — 메타인지적 도구 사용 (갱신)
- [[sources/2026-04-13-visually-grounded-humanoid-agents.md|Visually-grounded Humanoid Agents]] (2026-04-13) — 시각 기반 휴머노이드 에이전트
