# Transformer

**카테고리**: AI/ML
**관련 논문**: 26편

## 정의

_Wiki 축적 중 (claude 분석 대기)_


## 논문에서 발견된 핵심 인사이트

- LLM의 임베딩 공간에서 mask token을 프로브로 활용하면, 별도 draft 모델 없이도 training-free로 multi-token prediction이 가능하며 이는 speculative decoding의 실용적 장벽을 크게 낮춘다.
- IMU 기반 자기운동 데이터를 MLLM에 통합함으로써 무거운 3D 재구성 없이도 물리적으로 그라운딩된 효율적 3D 공간 추론이 가능하다.
- Transformer 아키텍처를 3D 장면의 6-DOF 물체 조작 궤적 합성에 적용하여, 멀티모달 장면 이해와 목표 조건부 제어를 통해 물리적으로 타당한 로봇 궤적 생성을 가능하게 한 프레임워크이다.
- 단안 비디오만으로 2D VLM에 명시적 3D 공간 추론 능력을 부여함으로써, 기하학적 단서를 보조 입력으로 추가하는 기존 접근법의 한계를 넘어 언어 기반 3D 위치 추정과 공간 추론을 통합한 프레임워크를 제시했다.
- 3D 형상 토큰화에서 기하학적 세부 수준(LoD) 대신 의미론적 계층(Level of Semantics)을 사용하면 토큰 효율성과 생성 품질을 동시에 개선할 수 있다.
- Galerkin 투영과 신경망 기저 함수를 결합하여 무한 차원 PIDE를 유한 차원 ODE로 축소함으로써, 시공간 제어 시스템의 고속 서로게이트 모델링을 실현한 연산자 학습 프레임워크이다.
- 텍스트 임베딩 공간에서의 단순 보간만으로 추가 학습 없이 연속적이고 제어 가능한 이미지 편집이 가능하며, 이는 멀티모달 모델의 임베딩 공간이 이미 시각적 속성 변화에 대해 충분히 구조화되어 있음을 보여준다.
- ViT와 LLM을 분리하지 않고 통합된 시공간 토큰 스코어링으로 비디오 VLM의 계산 효율성을 달성한 점이 핵심이며, 이는 기존 단일 단계 프루닝의 정보 손실 문제를 해결한다.
- 비디오를 계층적 그리드로 표현함으로써 장시간 비디오 이해를 로그 스케일 연산으로 축소하고, 캡션 없이도 시각적 충실도를 보존하는 무손실 탐색이 가능하다.
- LLM은 next-token prediction으로만 훈련되었음에도 임베딩 공간 프로빙만으로 훈련 없이 다중 토큰 병렬 예측이 가능하며, 이는 드래프트 모델 없는 speculative decoding을 실현한다.
- 단안 비디오만으로 2D VLM에 3D 공간 추론 능력을 부여함으로써, 별도 깊이 센서 없이도 언어 기반 로컬라이제이션과 시점 인식 추론이 가능해진다.
- ViT와 LLM을 관통하는 통합 시공간 토큰 스코어링으로, 비디오 VLM에서 시간적·공간적 중복 토큰을 동시에 제거하여 효율성과 성능을 양립시킨다.
- 비디오를 계층적 그리드로 표현함으로써 캡션 변환 없이 무손실 시각 정보를 로그 복잡도로 탐색할 수 있어, 장시간 비디오 이해의 효율성과 충실도를 동시에 달성한다.
- LLM 안전성을 사후 행동 교정(RLHF, 필터링)이 아닌 추론 프로세스 자체의 아키텍처적 제어로 전환함으로써, 환각과 적대적 공격에 대한 구조적 방어를 실현하려는 새로운 패러다임을 제시한다.
- GPU 커널 최적화 벤치마크를 소프트웨어 베이스라인 대비 상대적 속도 향상이 아닌, 하드웨어 이론적 성능 한계(Speed-of-Light) 대비 절대적 효율로 평가하는 패러다임 전환을 제안한다.

## 전체 관련 논문 (26편)

- [[sources/2026-03-19-efficient-training-free-multi-token-prediction-via.md|2026 03 19 efficient training free multi token prediction via.md]] (2026-03-19)
- [[sources/2026-03-19-feeling-the-space-egomotion-aware-video-representa.md|2026 03 19 feeling the space egomotion aware video representa.md]] (2026-03-19)
- [[sources/2026-03-19-gmt-goal-conditioned-multimodal-transformer-for-6-.md|2026 03 19 gmt goal conditioned multimodal transformer for 6 .md]] (2026-03-19)
- [[sources/2026-03-19-loc3r-vlm-language-based-localization-and-3d-reaso.md|2026 03 19 loc3r vlm language based localization and 3d reaso.md]] (2026-03-19)
- [[sources/2026-03-19-lost-level-of-semantics-tokenization-for-3d-shapes.md|2026 03 19 lost level of semantics tokenization for 3d shapes.md]] (2026-03-19)
- [[sources/2026-03-19-rhyme-xt-a-neural-operator-for-spatiotemporal-cont.md|2026 03 19 rhyme xt a neural operator for spatiotemporal cont.md]] (2026-03-19)
- [[sources/2026-03-19-the-unreasonable-effectiveness-of-text-embedding-i.md|2026 03 19 the unreasonable effectiveness of text embedding i.md]] (2026-03-19)
- [[sources/2026-03-19-unified-spatio-temporal-token-scoring-for-efficien.md|2026 03 19 unified spatio temporal token scoring for efficien.md]] (2026-03-19)
- [[sources/2026-03-19-videoatlas-navigating-long-form-video-in-logarithm.md|2026 03 19 videoatlas navigating long form video in logarithm.md]] (2026-03-19)
- [[sources/2026-03-20-efficient-training-free-multi-token-prediction-via.md|2026 03 20 efficient training free multi token prediction via.md]] (2026-03-20)
- [[sources/2026-03-20-loc3r-vlm-language-based-localization-and-3d-reaso.md|2026 03 20 loc3r vlm language based localization and 3d reaso.md]] (2026-03-20)
- [[sources/2026-03-20-unified-spatio-temporal-token-scoring-for-efficien.md|2026 03 20 unified spatio temporal token scoring for efficien.md]] (2026-03-20)
- [[sources/2026-03-20-videoatlas-navigating-long-form-video-in-logarithm.md|2026 03 20 videoatlas navigating long form video in logarithm.md]] (2026-03-20)
- [[sources/2026-03-21-box-maze-a-process-control-architecture-for-reliab.md|2026 03 21 box maze a process control architecture for reliab.md]] (2026-03-21)
- [[sources/2026-03-22-sol-execbench-speed-of-light-benchmarking-for-real.md|2026 03 22 sol execbench speed of light benchmarking for real.md]] (2026-03-22)
- [[sources/2026-03-25-chimera-latency--and-performance-aware-multi-agent.md|2026 03 25 chimera latency  and performance aware multi agent.md]] (2026-03-25)
- [[sources/2026-03-26-vision-on-request-enhanced-vllm-efficiency-with-sp.md|2026 03 26 vision on request enhanced vllm efficiency with sp.md]] (2026-03-26)
- [[sources/2026-03-27-chameleon-episodic-memory-for-long-horizon-robotic.md|2026 03 27 chameleon episodic memory for long horizon robotic.md]] (2026-03-27)
- [[sources/2026-04-03-leo-graph-attention-network-based-hybrid-multi-sen.md|2026 04 03 leo graph attention network based hybrid multi sen.md]] (2026-04-03)
- [[sources/2026-04-03-universal-yoco-for-efficient-depth-scaling.md|2026 04 03 universal yoco for efficient depth scaling.md]] (2026-04-03)
- [[sources/2026-04-04-steerable-visual-representations.md|2026 04 04 steerable visual representations.md]] (2026-04-04)
- [[sources/2026-04-05-steerable-visual-representations.md|2026 04 05 steerable visual representations.md]] (2026-04-05)
- [[sources/2026-04-06-steerable-visual-representations.md|2026 04 06 steerable visual representations.md]] (2026-04-06)
- [[sources/2026-04-09-in-place-test-time-training.md|2026 04 09 in place test time training.md]] (2026-04-09)
- [[sources/2026-04-09-toward-consistent-world-models-with-multi-token-pr.md|2026 04 09 toward consistent world models with multi token pr.md]] (2026-04-09)
- [[sources/2026-04-13-psi-shared-state-as-the-missing-layer-for-coherent.md|2026 04 13 psi shared state as the missing layer for coherent.md]] (2026-04-13)

- [[sources/2026-04-18-how-do-llms-and-vlms-understand-viewpoint-rotation.md]]

- [[sources/2026-04-19-how-do-llms-and-vlms-understand-viewpoint-rotation.md]]
