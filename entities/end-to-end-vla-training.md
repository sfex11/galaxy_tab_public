# end-to-end-vla-training

**카테고리**: 미분류
**생성일**: 2026-09-06

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-06-continuous-actions-from-discrete-minds-latent-alig.md|Continuous Actions from Discrete Minds: Latent-Aligned Plann]]

### A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia (2026-09-07)

command-conditioned behavior cloning이라는 최소 구성의 end-to-end 기준선을 제공하여, VLA 계열 연구([[Continuous Actions from Discrete Minds]])가 자율주행 도메인에서 요구하는 최소 검증 환경을 구체화한다. 정책 학습의 하한선 정의라는 점에서 잠재 정렬 등 고급 기법의 개선 폭을 측정하는 베이스라인 역할을 수행한다.

### Continuous Actions from Discrete Minds: Latent-Aligned Planning for En (2026-09-07)

잔여 VQ-VAE 액션 토크나이저로 차량 운동학을 이산 토큰화함으로써, VLA 종단간 훈련이 로봇 조작에서 자율주행이라는 연속·물리제약 도메인으로 확장 가능함을 실증한다. VLA 훈련 패러다임의 도메인 불변성을 검증하는 테스트 케이스가 된다.

### OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre (2026-09-19)

오픈루프 행동 복제 사전학습과 폐루프 온폴리시 파인튜닝의 이단계 구조를 제시하여, end-to-end 정책 훈련이 사전학습-사후학습의 연속체임을 자율주행에서 구체화한다.

### OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre (2026-09-21)

종단간 주행 정책의 2단계 라이프사이클 — BC 개루프 사전학습 → 온폴리시 폐루프 포스트트레이닝 — 을 확립한다. 미니어처 플랫폼의 command-conditioned BC 기준선 위에 놓이는 개선 계층이다.

→ [[sources/2026-09-21-opted-on-policy-fine-tuning-for-end-to-end-driving.md|상세 보기]]

### SeeQ: Training Generalist Value Functions for Long-Horizon Robotic Man (2026-09-22)

VLA 정책 개선에 외부 가치 함수가 후보 행동을 순위화하는 결합 계층을 추가한다. end-to-end 훈련이 정책 단독 최적화를 넘어 정책-가치 결합 구조를 포괄함을 시사한다.

→ [[sources/2026-09-22-seeq-training-generalist-value-functions-for-long-.md|상세 보기]]

### PRIME: Perception Feedback with Situational Memory Embeddings in VLA M (2026-09-22)

PRIME는 종단간 VLA의 피드포워드 구조 자체가 지각의 맹목성을 낳는다고 진단하고, 계획→지각 학습 피드백으로 위계 내부에 폐루프를 삽입한다. end-to-end의 정의를 '단방향 단일 파이프라인'에서 '양방향 정보 흐름을 갖는 파이프라인'으로 확장한다.

→ [[sources/2026-09-22-prime-perception-feedback-with-situational-memory-.md|상세 보기]]

### TANDEM: Task and Motion Planning with As-Needed Demonstrations for Eff (2026-09-25)

TANDEM은 VLA 미세조정의 데이터 수집 병목에 대한 해법을 제공한다 — TAMP가 자율 수행 가능 행동의 시연을 자동화하고 인간 시연을 계획 커버리지 밖 구간으로 한정하여, 훈련 파이프라인 축과 별도로 데이터 획득 축의 효율화 경로를 연다.

→ [[sources/2026-09-25-tandem-task-and-motion-planning-with-as-needed-dem.md|상세 보기]]
