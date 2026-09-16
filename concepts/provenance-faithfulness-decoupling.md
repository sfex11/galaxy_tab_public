# 프로버넌스-충실성 분리 (트레이스 3계층 신뢰 모델)

**생성일**: 2026-09-16

## 정의

트레이스 신뢰성을 ①출처·무결성(이 트레이스가 실제 그 실행에서 산출되었는가 — 인증 가능), ②충실성(진짜 트레이스가 내부 계획을 충실히 반영하는가 — 인증으로 해결 불가), ③안전성(반영된 계획이 안전한가 — 모니터 영역)의 3계층으로 분리하는 신뢰 모델. Plan injection은 ②(인증 부재 시 ①까지)를 깨뜨리며, ①을 완벽히 인증해도 ②는 여전히 열려 있다는 비환원성이 핵심.

## 관련 논문

- agent-execution-semantic-opacity
- cot-monitorability
- plan-injection
- plan-trace-separation
- alignment-base-opacity

---
_자동 Wiki Query에서 추출됨_
