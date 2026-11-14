# behavior-infrastructure-dual-cost-model

**카테고리**: 미분류
**생성일**: 2026-09-30

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-09-30-tokencast-forecasting-token-consumption-during-llm.md|TokenCast: Forecasting Token Consumption During LLM Agent Ex]]

### The SIMPLE Law for Energy Cost of LLM Inference (2026-11-04)

행동-인프라 곱셈 비용 모델에 '시퀀스 내 위치'라는 제3 차원을 추가한다. 동일 호출 횟수라도 누적 컨텍스트가 길수록 호출당 비용이 상승하므로, (기본 비용+오버헤드)×호출 횟수의 선형 구조가 컨텍스트 축적 하에서 초선형으로 변형됨이 해석적으로 정당화된다.

### CoReMem: Cost-Internalizing Memory for Successive Coding Tasks with Pr (2026-11-14)

행동-인프라 비용 모델에 메모리 쓰기-읽기 비용 축을 추가한다. 쓰기(인프라 투자)와 읽기(행동 시 비용)의 시점 분리된 결합 구조를 규정한다.

→ [[sources/2026-11-14-coremem-cost-internalizing-memory-for-successive-c.md|상세 보기]]
