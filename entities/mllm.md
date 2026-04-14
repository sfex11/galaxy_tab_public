# Mllm

**카테고리**: AI/ML
**관련 논문**: 21편

## 정의

_Wiki 축적 중 (claude 분석 대기)_


## 논문에서 발견된 핵심 인사이트

- 단안 비디오만으로 2D VLM에 명시적 3D 공간 추론 능력을 부여함으로써, 기하학적 단서를 보조 입력으로 추가하는 기존 접근법의 한계를 넘어 언어 기반 3D 위치 추정과 공간 추론을 통합한 프레임워크를 제시했다.
- 비디오 생성 모델이 학습 과정에서 자연스럽게 획득한 암묵적 3D 공간 프라이어를 명시적 3D 데이터 없이 장면 이해에 전이할 수 있다는 패러다임 전환을 제시한다.
- 체화된 내비게이션 시스템의 실환경 배포를 위해, 이상적 조건이 아닌 체계적 입력 손상 하에서의 신뢰성 평가가 필수적이며, NavTrust는 VLN과 OGN을 통합하는 최초의 강건성 벤치마크를 제시한다.
- MARCUS는 에이전틱 VLM 패러다임을 임상 심장학에 적용하여, 이질적 의료 모달리티(ECG/초음파/MRI)를 통합 추론하는 대화형 진단 시스템을 구현함으로써 도메인 특화 멀티모달 에이전트의 실현 가능성을 입증했다.
- 멀티모달 LLM을 실내/객체 수준에서 도시 규모 3D 환경으로 확장하기 위해 coarse-to-fine 병렬 브랜치 인코딩과 자동화된 대규모 데이터 생성 파이프라인을 결합한 최초의 통합 프레임워크를 제안했다.
- speculative decoding의 '추측 후 검증' 패러다임을 토큰 수준에서 에이전트 파이프라인 수준으로 확장하여, 멀티모달 에이전트의 인식-추론-도구호출 루프를 병렬화하는 새로운 가속 계층을 제시했다.
- 시각 토큰을 제거하는 대신 레이어별 시각-언어 상호작용을 동적으로 선택함으로써, 정보 손실 없이 LVLM 추론 효율을 개선할 수 있다는 새로운 패러다임을 제시한다.
- 로봇 조작에서 의미 압축 기반 메모리 대신 원시 지각 단서를 보존하는 에피소딕 메모리가 관찰 수준의 비마르코프 의사결정 문제를 효과적으로 해결한다.
- 실패 궤적을 단순 거부하지 않고 credit assignment를 통해 학습 신호로 재활용함으로써, 희소 보상 환경의 장기 호라이즌 GUI 태스크에서 에이전트의 자기진화를 가능하게 한다.
- MLLM의 자기 불확실성(엔트로피)을 글로벌 토큰 선택과 적응적 조기 종료의 제어 신호로 활용함으로써, 학습 없이도 장기 비디오 이해의 효율성과 성능을 동시에 달성할 수 있다.
- 단일 이미지·단일 턴 평가를 넘어, 시각적으로 유사한 다중 이미지 갤러리에서 순차적 질문 전략을 통해 타겟을 식별하는 장기 지평 벤치마크를 최초로 제안하여 에이전틱 VLM의 능동적 추론 능력을 체계적으로 측정할 수 있게 했다.
- VLA 모델에서 공간 인지와 의미 추론의 트레이드오프를 통합 아키텍처로 해결하여, 자율주행 VLA가 2D 언어 지식과 3D 공간 정보를 동시에 활용할 수 있는 경로를 제시한다.
- VLN 에이전트의 비효율적 탐색(진동, 재방문)은 단순한 계획 알고리즘 문제가 아니라 메타인지 능력의 부재에서 비롯되며, 자기 모니터링과 전략 진단 메커니즘을 도입함으로써 training-free 환경에서도 탐색 효율을 크게 개선할 수 있다.
- ViT의 범용 시각 특징을 텍스트 조건부 경량 어댑터로 조종함으로써, MLLM의 언어 중심성과 순수 ViT의 비유도성 사이의 간극을 메우는 새로운 표현 패러다임을 제시한다.
- RL 후훈련이 MLLM의 시각적 추론을 향상시키는 것처럼 보이지만, 실제로는 시각 정보 활용 없이 텍스트 패턴 기반 환각에 의존한 추론 단축을 학습할 수 있으며, 이는 보상 해킹의 멀티모달 변형이다.

## 전체 관련 논문 (21편)

- [[sources/2026-03-19-loc3r-vlm-language-based-localization-and-3d-reaso.md|2026 03 19 loc3r vlm language based localization and 3d reaso.md]] (2026-03-19)
- [[sources/2026-03-22-generation-models-know-space-unleashing-implicit-3.md|2026 03 22 generation models know space unleashing implicit 3.md]] (2026-03-22)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md|2026 03 23 navtrust benchmarking trustworthiness for embodied.md]] (2026-03-23)
- [[sources/2026-03-25-marcus-an-agentic-multimodal-vision-language-model.md|2026 03 25 marcus an agentic multimodal vision language model.md]] (2026-03-25)
- [[sources/2026-03-26-3dcity-llm-empowering-multi-modality-large-languag.md|2026 03 26 3dcity llm empowering multi modality large languag.md]] (2026-03-26)
- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md|2026 03 26 speceyes accelerating agentic multimodal llms via .md]] (2026-03-26)
- [[sources/2026-03-26-vision-on-request-enhanced-vllm-efficiency-with-sp.md|2026 03 26 vision on request enhanced vllm efficiency with sp.md]] (2026-03-26)
- [[sources/2026-03-27-chameleon-episodic-memory-for-long-horizon-robotic.md|2026 03 27 chameleon episodic memory for long horizon robotic.md]] (2026-03-27)
- [[sources/2026-03-27-ui-voyager-a-self-evolving-gui-agent-learning-via-.md|2026 03 27 ui voyager a self evolving gui agent learning via .md]] (2026-03-27)
- [[sources/2026-03-31-adapttoken-entropy-based-adaptive-token-selection-.md|2026 03 31 adapttoken entropy based adaptive token selection .md]] (2026-03-31)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md|2026 04 01 amigo agentic multi image grounding oracle benchma.md]] (2026-04-01)
- [[sources/2026-04-03-unidrivevla-unifying-understanding-perception-and-.md|2026 04 03 unidrivevla unifying understanding perception and .md]] (2026-04-03)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md|2026 04 04 stop wandering efficient vision language navigatio.md]] (2026-04-04)
- [[sources/2026-04-05-steerable-visual-representations.md|2026 04 05 steerable visual representations.md]] (2026-04-05)
- [[sources/2026-04-07-understanding-the-role-of-hallucination-in-reinfor.md|2026 04 07 understanding the role of hallucination in reinfor.md]] (2026-04-07)
- [[sources/2026-04-09-mmemb-r1-reasoning-enhanced-multimodal-embedding-w.md|2026 04 09 mmemb r1 reasoning enhanced multimodal embedding w.md]] (2026-04-09)
- [[sources/2026-04-11-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|2026 04 11 openvlthinkerv2 a generalist multimodal reasoning .md]] (2026-04-11)
- [[sources/2026-04-12-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 12 act wisely cultivating meta cognitive tool use in .md]] (2026-04-12)
- [[sources/2026-04-12-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|2026 04 12 openvlthinkerv2 a generalist multimodal reasoning .md]] (2026-04-12)
- [[sources/2026-04-13-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 13 act wisely cultivating meta cognitive tool use in .md]] (2026-04-13)
- [[sources/2026-04-13-visually-grounded-humanoid-agents.md|2026 04 13 visually grounded humanoid agents.md]] (2026-04-13)
