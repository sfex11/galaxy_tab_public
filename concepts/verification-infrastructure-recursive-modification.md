# 검증 인프라의 재귀적 재작성

**생성일**: 2026-09-03

## 정의

동적 하네스에서 에이전트의 컴포넌트 변경이 롤백·분기의 근거인 의존 그래프 자체를 재작성하여, 검증 인프라(C/R 런타임)가 검증 대상 내부로 들어오는 재귀 구조. 안전망이 계속 기능하려면 변경 전후 의존 구조 변화를 정확히 기술하는 파급 추론이 전제된다.

## 관련 논문

- checkpoint-restore-efficiency-spectrum
- recursive-checkpoint-scope-problem
- harness-mutability
- algorithm-system-translation-gap

---
_자동 Wiki Query에서 추출됨_
