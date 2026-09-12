# adaptive-inference

**카테고리**: 미분류
**생성일**: 2026-05-05

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-05-to-call-or-not-to-call-a-framework-to-assess-and-o.md|To Call or Not to Call: A Framework to Assess and Optimize L]]

### SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel (2026-05-05)

적응적 추론의 결정 차원을 모델/라우트 선택에서 추측 길이(γ) 선택으로 확장한다. 기존 컨텍스트 기반 적응(CADENCE 등)이 외부 환경에 반응했다면, SpecKV는 압축이라는 내부 시스템 상태에 반응하는 적응의 새로운 유형을 제시한다.

### SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel (2026-05-06)

적응의 결정 차원을 모델/라우트 선택에서 추측 길이(γ) 선택으로 확장한다. 기존 컨텍스트 기반 적응(CADENCE 등)이 외부 환경에 반응했다면, SpecKV는 압축이라는 내부 시스템 상태에 반응하는 적응의 새로운 유형을 제시한다.

### LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agen (2026-05-08)

적응적 추론의 결정 차원을 모델/라우트 선택, 추측 길이(γ)에서 컨텍스트 상세도(detail level)로 확장한다. 기존 컨텍스트 기반 적응(CADENCE 등)이 외부 환경에 반응했다면, LongSeeker은 에이전트 자신의 궤적 내부에서 현재 관련도에 따라 정보의 충실도를 차등적으로 조절하는 내적 적응의 새로운 유형을 제시한다.

### Recursive Agent Optimization (2026-05-10)

RAO는 기존 적응적 추론이 주로 계산 자원 축소(하향식)에 집중한 한계를 교정하여, 문제 복잡도에 맞춰 자기 재귀적으로 자원을 확장하는 상향식 적응 경로를 최초로 훈련 가능한 형태로 구현하여 적응적 추론의 스펙트럼을 양방향으로 완성한다.

### EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction (2026-09-04)

적응적 계산의 결정 차원을 배포 시점(추측 길이 γ, 라우트 선택)에서 평가 시점(궤적 지속 여부)으로 확장한다. SpecKV가 내부 압축 상태에 반응했다면, EarlyEval은 조기 예측된 결과의 확신도에 반응해 계산을 중단하되, 적응 주체가 모델이 아닌 평가 하네스이며 중단이 측정 충실도를 훼손하지 않아야 한다는 제약이 결합된 새로운 적응 유형임을 보여준다.

### ShallowStream: Index Shallow then Answer Deep for Streaming Video Unde (2026-09-04)

적응의 트리거 축에 '질의 도착 이벤트'라는 제4유형을 추가한다. 외부 환경 반응(CADENCE), 내부 시스템 상태 반응(SpecKV)과 달리, ShallowStream은 질의 도착 전후로 계산 깊이 자체를 이단계로 분리하는 구조적 적응을 보여준다.

### Efficient Test-Time Adaptation through Human-AI Interaction (2026-09-06)

적응적 추론의 반응 대상 스펙트럼에 '인간 상호작용에서 발현되는 암묵적 개인 기준'이라는 제4유형을 추가한다. 외부 환경(CADENCE)·내부 시스템 상태(SpecKV)·신념 상태에 이어, 사용자와의 반복 교환을 통한 기준 표면화가 테스트 시점 적응의 새로운 결정 차원임을 보여준다.

### Trust-Aware Adaptive Disclosure for Inference Privacy Preservation in  (2026-09-08)

적응의 결정 차원을 계산량·내부 상태에서 '정보 공개 수준'으로 확장하는 사례를 제공한다 — 신뢰 상태에 반응해 공개를 조절하는 것은 사회적 상태 반응형 적응이라는 새로운 유형이다.

→ [[sources/2026-09-08-trust-aware-adaptive-disclosure-for-inference-priv.md|상세 보기]]

### Don't Drop Dropout: Optimizing Layer Sparsity for Efficient LLM Traini (2026-09-08)

추론의 적응 축에 아키텍처 깊이 축을 새로 추가한다. SpecKV의 내부 상태 반응과 CADENCE의 외부 컨텍스트 반응이 고정 아키텍처 내에서 작동했다면, 계층 수준 탄력성은 모델 깊이 자체의 런타임 선택을 가능하게 하여 [[token-pruning]]의 깊이축 확장이다.

→ [[sources/2026-09-08-dont-drop-dropout-optimizing-layer-sparsity-for-ef.md|상세 보기]]

### Beyond One-Size-Fits-All: Sample-Adaptive Strategy Routing for Vision  (2026-09-11)

적응의 결정 차원에 제3의 축을 추가한다. 기존 확장이 외부 환경 반응(CADENCE)과 내부 시스템 상태 반응(SpecKV)이었다면, 본 논문은 입력 샘플에 대한 알고리즘·전략 선택이라는 새로운 적응 유형을 제시하여, 적응 대상이 파라미터 튜닝에서 알고리즘 간 라우팅으로 격상됨을 보여준다.

→ [[sources/2026-09-11-beyond-one-size-fits-all-sample-adaptive-strategy-.md|상세 보기]]

### Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware A (2026-09-12)

적응의 결정 차원을 계산량 조절(토큰 예산, 압축률)에서 모달리티 선택으로 확장한다. '얼마나 계산할까'가 아닌 '언제 시각적으로 볼까'는 토큰 수준 적응과 직교하는 새로운 적응 축이며, 시각 필요성 판별이라는 내부 인지 상태 기반 적응 유형으로 분류된다.

→ [[sources/2026-09-12-caption-once-frames-on-demand-visual-need-routing-.md|상세 보기]]

### RetroThinker: Enabling Retrospective Thinking in Speech LLMs (2026-09-12)

적응의 결정 축에 '언제 계산하는가(출력 이전 vs 이후)'라는 시간 배치 차원을 추가한다. 기존 정의가 예산·라우팅·궤적 축의 적응을 다뤘다면, 회고적 추론은 추론 연산의 출력 대비 위치 자체를 적응 대상으로 삼아 지연 민감 도메인에서 사고-응답 순서가 자유로운 설계 변수임을 보여준다.

→ [[sources/2026-09-12-retrothinker-enabling-retrospective-thinking-in-sp.md|상세 보기]]
