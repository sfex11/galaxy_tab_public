# Vlm

**카테고리**: AI/ML
**관련 논문**: 26편

## 정의

_Wiki 축적 중 (claude 분석 대기)_


## 논문에서 발견된 핵심 인사이트

- 단안 비디오만으로 2D VLM에 명시적 3D 공간 추론 능력을 부여함으로써, 기하학적 단서를 보조 입력으로 추가하는 기존 접근법의 한계를 넘어 언어 기반 3D 위치 추정과 공간 추론을 통합한 프레임워크를 제시했다.
- 단안 비디오만으로 2D VLM에 3D 공간 추론 능력을 부여함으로써, 별도 깊이 센서 없이도 언어 기반 로컬라이제이션과 시점 인식 추론이 가능해진다.
- 체화된 내비게이션 에이전트의 평가를 이상적 조건의 성능 측정에서 실세계 입력 손상에 대한 신뢰성 평가로 확장하여, 안전한 실배포를 위한 벤치마크 패러다임을 제시한다.
- 비디오 생성 모델이 학습 과정에서 자연스럽게 획득한 암묵적 3D 공간 프라이어를 명시적 3D 데이터 없이 장면 이해에 전이할 수 있다는 패러다임 전환을 제시한다.
- VLM의 의미적 그라운딩 능력과 물리적 메트릭 추론을 다중 에이전트 확률적 프레임워크로 분리·통합함으로써, 로봇 내비게이션에서 정밀한 공간 명령 수행이 가능해진다.
- NavTrust는 체화된 내비게이션 모델을 이상적 조건이 아닌 실세계 손상 시나리오에서 평가함으로써, 성능 중심 평가에서 신뢰성 중심 평가로의 전환을 제안하는 최초의 통합 벤치마크이다.
- VLM의 의미적 그라운딩 능력과 메트릭 공간 추론의 간극을 다중 에이전트 확률적 프레임워크로 연결함으로써, 자연어 명령의 물리적 실행 가능성을 크게 높였다.
- 체화된 내비게이션 시스템의 실환경 배포를 위해, 이상적 조건이 아닌 체계적 입력 손상 하에서의 신뢰성 평가가 필수적이며, NavTrust는 VLN과 OGN을 통합하는 최초의 강건성 벤치마크를 제시한다.
- 장면 그래프 위에서의 구조적 추론을 통해 LLM/VLM의 공간 이해 한계를 극복하고, 자연어 지시 기반의 정밀한 3D 레이아웃 편집을 가능하게 한 점이 핵심이다.
- MARCUS는 에이전틱 VLM 패러다임을 임상 심장학에 적용하여, 이질적 의료 모달리티(ECG/초음파/MRI)를 통합 추론하는 대화형 진단 시스템을 구현함으로써 도메인 특화 멀티모달 에이전트의 실현 가능성을 입증했다.
- 멀티모달 LLM을 실내/객체 수준에서 도시 규모 3D 환경으로 확장하기 위해 coarse-to-fine 병렬 브랜치 인코딩과 자동화된 대규모 데이터 생성 파이프라인을 결합한 최초의 통합 프레임워크를 제안했다.
- 시각 토큰을 제거하는 대신 레이어별 시각-언어 상호작용을 동적으로 선택함으로써, 정보 손실 없이 LVLM 추론 효율을 개선할 수 있다는 새로운 패러다임을 제시한다.
- 로봇 조작에서 의미 압축 기반 메모리 대신 원시 지각 단서를 보존하는 에피소딕 메모리가 관찰 수준의 비마르코프 의사결정 문제를 효과적으로 해결한다.
- 에이전틱 VLM 평가를 단일 턴 정답률에서 다중 턴 전략적 질문 생성과 정보 통합 능력 측정으로 전환함으로써, 실제 에이전트 배포 시나리오에 부합하는 평가 패러다임을 제시한다.
- 프론티어 포인트 대신 지속적 방향(persistent direction)을 탐색 단위로 사용하면, 불완전한 관측 하에서의 경로 불안정성과 반복 방문 문제를 구조적으로 해소할 수 있다.

## 전체 관련 논문 (26편)

- [[sources/2026-03-19-loc3r-vlm-language-based-localization-and-3d-reaso.md|2026 03 19 loc3r vlm language based localization and 3d reaso.md]] (2026-03-19)
- [[sources/2026-03-20-loc3r-vlm-language-based-localization-and-3d-reaso.md|2026 03 20 loc3r vlm language based localization and 3d reaso.md]] (2026-03-20)
- [[sources/2026-03-21-navtrust-benchmarking-trustworthiness-for-embodied.md|2026 03 21 navtrust benchmarking trustworthiness for embodied.md]] (2026-03-21)
- [[sources/2026-03-22-generation-models-know-space-unleashing-implicit-3.md|2026 03 22 generation models know space unleashing implicit 3.md]] (2026-03-22)
- [[sources/2026-03-22-meanings-and-measurements-multi-agent-probabilisti.md|2026 03 22 meanings and measurements multi agent probabilisti.md]] (2026-03-22)
- [[sources/2026-03-22-navtrust-benchmarking-trustworthiness-for-embodied.md|2026 03 22 navtrust benchmarking trustworthiness for embodied.md]] (2026-03-22)
- [[sources/2026-03-23-meanings-and-measurements-multi-agent-probabilisti.md|2026 03 23 meanings and measurements multi agent probabilisti.md]] (2026-03-23)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md|2026 03 23 navtrust benchmarking trustworthiness for embodied.md]] (2026-03-23)
- [[sources/2026-03-25-3d-layout-r1-structured-reasoning-for-language-ins.md|2026 03 25 3d layout r1 structured reasoning for language ins.md]] (2026-03-25)
- [[sources/2026-03-25-marcus-an-agentic-multimodal-vision-language-model.md|2026 03 25 marcus an agentic multimodal vision language model.md]] (2026-03-25)
- [[sources/2026-03-26-3dcity-llm-empowering-multi-modality-large-languag.md|2026 03 26 3dcity llm empowering multi modality large languag.md]] (2026-03-26)
- [[sources/2026-03-26-vision-on-request-enhanced-vllm-efficiency-with-sp.md|2026 03 26 vision on request enhanced vllm efficiency with sp.md]] (2026-03-26)
- [[sources/2026-03-27-chameleon-episodic-memory-for-long-horizon-robotic.md|2026 03 27 chameleon episodic memory for long horizon robotic.md]] (2026-03-27)
- [[sources/2026-03-31-amigo-agentic-multi-image-grounding-oracle-benchma.md|2026 03 31 amigo agentic multi image grounding oracle benchma.md]] (2026-03-31)
- [[sources/2026-03-31-drive-nav-directional-reasoning-inspection-and-ver.md|2026 03 31 drive nav directional reasoning inspection and ver.md]] (2026-03-31)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md|2026 04 01 amigo agentic multi image grounding oracle benchma.md]] (2026-04-01)
- [[sources/2026-04-03-unidrivevla-unifying-understanding-perception-and-.md|2026 04 03 unidrivevla unifying understanding perception and .md]] (2026-04-03)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md|2026 04 04 stop wandering efficient vision language navigatio.md]] (2026-04-04)
- [[sources/2026-04-05-steerable-visual-representations.md|2026 04 05 steerable visual representations.md]] (2026-04-05)
- [[sources/2026-04-06-stop-wandering-efficient-vision-language-navigatio.md|2026 04 06 stop wandering efficient vision language navigatio.md]] (2026-04-06)
- [[sources/2026-04-10-appear2meaning-a-cross-cultural-benchmark-for-stru.md|2026 04 10 appear2meaning a cross cultural benchmark for stru.md]] (2026-04-10)
- [[sources/2026-04-11-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|2026 04 11 openvlthinkerv2 a generalist multimodal reasoning .md]] (2026-04-11)
- [[sources/2026-04-12-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 12 act wisely cultivating meta cognitive tool use in .md]] (2026-04-12)
- [[sources/2026-04-12-openvlthinkerv2-a-generalist-multimodal-reasoning-.md|2026 04 12 openvlthinkerv2 a generalist multimodal reasoning .md]] (2026-04-12)
- [[sources/2026-04-13-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 13 act wisely cultivating meta cognitive tool use in .md]] (2026-04-13)
- [[sources/2026-04-13-visually-grounded-humanoid-agents.md|2026 04 13 visually grounded humanoid agents.md]] (2026-04-13)
