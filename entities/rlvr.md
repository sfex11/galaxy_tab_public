# rlvr

**카테고리**: 미분류
**생성일**: 2026-09-04

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-04-cliff-learning-process-rewards-from-the-first-mist.md|Cliff: Learning Process Rewards from the First Mistake]]

### Post-Training Language Models for Gold-Medal Performance in Coding Com (2026-09-04)

코딩 경쟁이 테스트 케이스 통과라는 결정적 검증자를 갖춘 RLVR의 전형적·최고난도 도메인임을 확인시킨다. 검증 가능성이 완전한 도메인에서조차 RL의 기여는 모델 스케일에 따라 달라진다는 스케일 조건부 구조를 추가한다.

### Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E (2026-09-06)

검증 가능 보상의 전제인 재질의 가능한 태스크 원천을 기존 궤적에서 파생시켜, RLVR의 확장성 제약을 수작업 환경 구축에서 궤적 자원 활용으로 전환한다.

### Environment Evolution for Terminal Agents (2026-09-06)

검증 가능 환경의 스케일링이 RLVR의 핵심 전제임을 재확인하고, 검증 가능성을 유지한 채 난이도를 지속적으로 재조정하는 환경 진화를 RLVR 인프라의 필수 구성요소로 격상시킨다.

### Terminal-Universe: Turning Agent Trajectories into Scalable Terminal E (2026-09-07)

RLVR의 검증 가능 태스크 부족 병목에 대한 공급 측 해법을 제공한다. 궤적을 소모성 SFT 데이터로 소비하는 대신 재질의 가능한 검증 태스크 생성기로 변환함으로써, 학습 신호의 공급량을 궤적 축적량에 연동한다.

### ExecCritic: Learn to Test, Test to Improve for Coding Agents (2026-09-10)

검증 가능 보상의 신호 품질이 테스트의 행동 커버리지에 의존함을 보여, RLVR의 '검증 가능성'이 고정 자산이 아니라 훈련되어야 하는 능력임을 규명한다. 검증자 역할을 RL 학습 대상에 포함시키는 확장을 제시한다.

### ActReview: Rebuttal-Guided Training Data and Rubric Rewards for Action (2026-09-10)

rubric reward를 통해 검증 가능 보상의 적용 범위를 정답이 명확한 과제(코딩, 수학)에서 주관적 품질 판단 도메인(피어 리뷰)으로 확장한다. 루브릭 형식화가 ground truth 부재를 우회하는 경로를 제시하나 상대적 검증의 한계를 그대로 계승한다.

### Bellman Policy Optimization (2026-09-16)

RLVR 파이프라인에서 상태 가치 추정 계층이 이론적으로 불필요할 수 있음을 증명하여, GRPO 계열 크리틱 프리 설계에 대한 이론적 정당화 근거를 제공한다.

### ScienceIDE: Turning World's Scientific Codebase into Agent Learnable E (2026-09-18)

검증 가능 훈련의 도메인 확장 근거를 제공한다. 과학 코드의 특수 정확성 기준이 실행 검증으로 형식화될 수 있음을 보여, RLVR이 수학·코딩 경쟁을 넘어 과학 컴퓨팅 도메인으로 확장될 수 있는 조건을 명시한다.

### Designer-RSI: Evolving Procedural Memory from User Traffic for Agentic (2026-09-22)

검증 가능 보상이 부재한 창작 도메인에서 개선이 어떻게 지속되는지의 대조 사례를 제공한다. RLVR 부재가 자기 개선의 병목이 아니라 신호 원천 전환(사용자 행동)의 동기가 됨을 시사한다.

→ [[sources/2026-09-22-designer-rsi-evolving-procedural-memory-from-user-.md|상세 보기]]

### CodeMidas: Scaling Agentic Coding RL Environments from Code Itself (2026-09-22)

신뢰할 수 있는 검증자를 갖춘 다양한 태스크 공급이라는 RLVR의 전제 조건을 코드베이스 자체에서 충족하는 경로를 제공한다. 검증 가능성이 외부 벤치마크의 속성이 아니라 코드의 실제 실행 가능성에서 유래함을 보여준다.

→ [[sources/2026-09-22-codemidas-scaling-agentic-coding-rl-environments-f.md|상세 보기]]
