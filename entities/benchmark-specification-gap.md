# benchmark-specification-gap

**카테고리**: 미분류
**생성일**: 2026-09-06

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-06-swe-gate-passing-functional-tests-is-not-enough-fo.md|SWE-Gate: Passing Functional Tests Is Not Enough for Softwar]]

### SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineer (2026-09-07)

벤치마크가 명세하지 않은 차원(리뷰 제약)이 실제 수용을 결정한다는 발견으로, 벤치마크 명세의 불완전성이 평가 대상 자체를 왜곡함을 SWE 도메인에서 실증한다. 명세 간극이 '측정 누락'을 넘어 '수용 기준 누락'으로 확장됨을 보여준다.

### Molecular Déjà Vu: Digit-Level Retrieval of Published Values in Fronti (2026-09-08)

분자 속성 벤치마크가 예측 능력과 출판 수치 검색 능력 중 무엇을 측정하는지 명세하지 않아 정확도가 두 능력을 구별 불가능하게 통합함을 화학 도메인에서 실증한다. 명세 간극이 오염 감지 불가능성으로 이어지는 구체적 인과 경로를 제공한다.

### CUA-Universe: A Scalable and Dynamic Environment for Hybrid GUI+CLI Ag (2026-09-08)

OSWorld·AndroidWorld가 명세에서 누락한 CLI 모달리티가 실제 작업 효율성을 결정함을 보여, 명세 간극이 측정 누락을 넘어 에이전트 행동 패턴(GUI 몰입 비효율) 자체를 구조적으로 왜곡함을 입증한다.

### IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research-Idea  (2026-09-11)

측정 명세(벤치마크)의 불완전성 문제를 구현 명세(연구 방법) 도메인으로 확장한다 — 명세 불완전성이 어떤 대상을 왜곡하는가는 도메인 불변의 구조적 결함임을 보여준다.

### JarvisGUI: Towards Cross-Device GUI Agents with Dynamic Task Compositi (2026-09-11)

GUI 벤치마크가 명세하지 않은 크로스 디바이스 차원(중간 결과 이전, 공유 상태, 이종 조율)이 실제 사용 준비도를 결정함을 보여, 명세 간극이 측정 누락을 넘어 '준비도 과대평가'라는 배포 리스크로 직결됨을 입증한다.

### Vulnerability Localization Benchmark: Measuring Agentic Security Analy (2026-09-16)

사이버보안 평가의 명세 누락 사례를 제공한다. 기존 벤치마크들이 탐지·재현·수리만 명세하여 국소화 능력이 평가 대상에서 체계적으로 누락되어 있었음을 드러내며, 명세 간극이 도메인 특정 능력 축 전체를 은폐할 수 있음을 강화한다.

### Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulati (2026-09-19)

기존 로봇 조작 벤치마크가 안전 축을 명세하지 않은 명세 간극의 실례를 제공한다. 목표-장애물 쌍 명세는 조작 평가에 안전 제약 준수라는 제2의 측정 축을 도입한다.

### Value-Sensitive Delegation in Everyday AI Agent Use: Evidence from Ope (2026-09-22)

평가 체계가 태스크 완성도를 측정하는 동안 사용자는 Bounded Reach·Reviewability 같은 가치를 우선한다는 발견으로, 명세 간극에 '사용자 가치의 명세 부재'라는 새 차원을 추가한다. 평가 대상이 이미 초기 명세 단계에서 사용자의 실제 관심사와 어긋남을 야생 데이터로 실증한다.

→ [[sources/2026-09-22-value-sensitive-delegation-in-everyday-ai-agent-us.md|상세 보기]]

### SWE-Serve: Benchmarking Agentic Engineering For Production Inference S (2026-09-24)

레포 수준 SWE 벤치마크가 추론 서빙을 다루지 않는 커버리지 공백을 실증한다. 벤치마크 스펙 간극이 '기존 벤치마크의 미시 오차'가 아니라 '도메인 전체의 측정 부재'로 발현될 수 있음을 보여준다.

→ [[sources/2026-09-24-swe-serve-benchmarking-agentic-engineering-for-pro.md|상세 보기]]

### Measuring the Serving Stack Instead of the Model: Hidden Confounds in  (2026-09-24)

서빙 스택 구성이 벤치마크가 명세하지 않은 은닉 차원임을 보여준다. 동일 모델이라도 로컬 서빙 구성에 따라 측정되는 능력이 달라지므로, 평가 명세에 서빙 계층 고정·공개 조건이 포함되어야 함을 시사한다.

→ [[sources/2026-09-24-measuring-the-serving-stack-instead-of-the-model-h.md|상세 보기]]

### Metrics Failure in LLM-Based Code Vulnerability Repair: An Empirical S (2026-09-24)

지표의 바닥선 포화라는 새 변형을 추가한다. 벤치마크가 명세한 지표(컴파일률)가 태스크의 초기 상태에 의해 이미 달성되어 측정 자체가 무정보가 되는 경우로, 명세 간극이 '누락된 차원'에서 '포화된 기준선'으로 확장됨을 보여준다.

→ [[sources/2026-09-24-metrics-failure-in-llm-based-code-vulnerability-re.md|상세 보기]]

### Fine-Tuning LLMs for Translation: General Forgetting Mitigation Does N (2026-09-25)

망각 완화 평가의 명세 간극 사례를 제공한다. '일반 벤치마크 유지율'이라는 표준 평가 관행이 실제 보존 목표(태스크 특화 지시 수행)를 명세하지 못하며, 명세의 누락이 완화 기법 연구의 결론 전환을 유발할 수 있음을 실증한다. SWE-Gate의 테스트-수용 단절과 동형인 '유지율-실보존' 간극이다.

→ [[sources/2026-09-25-fine-tuning-llms-for-translation-general-forgettin.md|상세 보기]]
