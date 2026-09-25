# autonomous-driving

**카테고리**: 미분류
**생성일**: 2026-09-04

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-04-toward-robust-lidar-semantic-segmentation-for-real.md|Toward Robust LiDAR Semantic Segmentation for Real-World Dep]]

### A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia (2026-09-06)

기존 LiDAR 인지-배포 간극 중심의 논의에서 end-to-end 정책 연구를 위한 개방형 실험 인프라 차원을 추가한다. 미니어처 Ackermann 플랫폼이 고비용 산업 실험 없이도 시뮬레이션-실차 검증 루프를 구축 가능함을 보여준다.

### Corner Cases: Headland Coverage Path Planning for Autonomous Driving i (2026-09-06)

온로드 차선 추종 중심의 기존 논의에 오프로드 농경 커버리지라는 축을 추가한다. 경작지 주행의 목표가 경로 최적화가 아닌 면적 완전 커버리지임을 보여, 자율주행 계획 문제의 구조가 도메인에 따라 근본적으로 달라짐(경로 최적화 vs 커버리지 최적화)을 시사한다.

### Continuous Actions from Discrete Minds: Latent-Aligned Planning for En (2026-09-06)

LiDAR 지각 강건성(Toward Robust LiDAR Semantic Segmentation) 중심이던 스코프를 지각-계획-행동이 통합된 end-to-end VLA 프레임워크로 확장하며, 지각 연구와 행동 생성 연구가 자율주행에서 수렴하는 지점을 제공한다.

### A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Minia (2026-09-07)

기존 LiDAR 인지-배포 간극 중심의 논의에서 end-to-end 정책 연구를 위한 개방형 실험 인프라 차원을 추가한다. 미니어처 Ackermann 플랫폼이 고비용 산업 실험 없이도 시뮬레이션-실차 검증 루프를 구축 가능하게 하여, 자율주행 연구의 병목이 알고리즘이 아닌 실험 인프라 접근성에 있음을 시사한다.

### Corner Cases: Headland Coverage Path Planning for Autonomous Driving i (2026-09-07)

자율주행의 적용 영역을 도로 주행에서 농경지 헤드랜드로 확장하는 도메인 변주를 제공한다. 도로 주행과 다른 목표 함수(커버리지)와 평가 축(gap·overlap·경계 침범)을 요구함을 보여준다.

### Continuous Actions from Discrete Minds: Latent-Aligned Planning for En (2026-09-07)

엔드투엔드 자율주행에서 인지-계획-제어 통합이 VLM 기반으로 가능함을 보여주며, LiDAR 인지 강화([[concepts/autonomous-driving-perception.md|autonomous driving perception]])와 개방형 실험 플랫폼 연구와 결합하면 자율주행 VLA 스택의 방법-인프라 전체 지형이 완성된다.

### OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre (2026-09-19)

인지·계획·커버리지 논의에 이어 end-to-end 정책의 폐루프 사후학습 축을 추가한다. 렌더링 프리 훈련은 자율주행 폐루프 학습의 계산 비용 장벽을 낮추는 인프라 방향을 제시한다.

### OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre (2026-09-21)

폐루프 안전 문제를 학습 문제로 재정의한다 — 배포 시 분포 이탈 위험을 폐루포스트트레이닝으로 사전 완화하는 경로를 제공하여, 자율주행 연구가 인지-계획 성능에서 훈련-배포 분포 정렬로 축을 이동 중임을 보여준다.

→ [[sources/2026-09-21-opted-on-policy-fine-tuning-for-end-to-end-driving.md|상세 보기]]

### PRIME: Perception Feedback with Situational Memory Embeddings in VLA M (2026-09-22)

자율주행 VLA 연구에 '지각 피드백' 설계 축을 추가한다. feedforward 추론이 표준이던 end-to-end 주행에서, 상황 기억을 통한 하류 조건부 지각이 새로운 설계 변수가 됨을 제시한다.

→ [[sources/2026-09-22-prime-perception-feedback-with-situational-memory-.md|상세 보기]]

### TM-APR: Thermal Temporal-Memory Localization via Analytic Online Adapt (2026-09-24)

위치 인식(VPR)이 자율 항행의 전제조건임을 명시하며, 열화상 센서라는 극단적 조건 도메인으로의 확장 사례를 추가한다. 기존 end-to-end 주행·플랫폼 논의가 정책 학습에 집중했다면, 본 논문은 그 하위 전제인 장소 인식의 배포 가능성을 다룬다.

→ [[sources/2026-09-24-tm-apr-thermal-temporal-memory-localization-via-an.md|상세 보기]]

### AnchorReasoning: A Visual Grounding and Causal Reasoning Dataset in Lo (2026-09-25)

하드웨어 인프라(미니어처 오픈 플랫폼)와 훈련 방법(OPTED, PRIME)에 이어 '장기 꼬리 시나리오용 근거 감독 데이터'라는 제3의 인프라 축을 제공한다. end-to-end 주행 연구의 병목이 훈련 루프·하드웨어에서 감독 데이터 설계로 이동하고 있음을 보여준다.

→ [[sources/2026-09-25-anchorreasoning-a-visual-grounding-and-causal-reas.md|상세 보기]]
