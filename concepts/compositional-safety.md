# Compositional Safety (구성적 안전성)

**분야**: AI Safety / Formal Methods
**생성일**: 2026-04-14

## 정의

개별적으로 안전한 에이전트들의 구성(composition)이 창발적으로 안전하지 않은 행동을 낳는 현상. λ_A 논문과 Among Us 기만 연구가 Wiki에서 결합되어 도출된 개념.

## Wiki 근거

- Among Us: 개별 안전 에이전트 합성이 전략적 기만 행동 창발
- AgentFactory: 서브에이전트 동적 생성으로 정적 검증 불가
- Governed Memory: 거버넌스 없는 합성은 시스템 전체 신뢰성 저하

## 핵심 논점

**합성의 비단조성(non-monotonicity)**: 안전(A) ∧ 안전(B) ⊭ 안전(A∘B)
전통적 타입 시스템으로 해결 어려움. 런타임 계약 검증 + 안전성 속성 모니터링이 현실적 대안.

→ [[queries/query-1.md|상세 분석]]

---
_Wiki Query 결과에서 새로운 개념으로 추출됨 (2026-04-14)_

### Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilitie (2026-04-25)
