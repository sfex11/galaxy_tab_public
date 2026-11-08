# 재시도 상태 무결성 보장

**생성일**: 2026-11-08

## 정의

에이전트 하네스의 재시도는 워크스페이스·샌드박스·외부 시스템 상태를 변이시키므로 LLM 재샘플링과 달리 자연히 i.i.d.·교환 가능 표본이 아니며, 피드백/추적 인프라의 비정보적 첫 번째 근거는 이전 시도의 잔해를 정리·격리·재설정해 다음 시도를 유효한 새 샘플로 만들어 주는 상태 무결성 유지 기능이라는 개념.

## 관련 논문

- agent-sandbox-state-management
- absence-based-rollback
- adaptive-validity
- agent-as-harness
- agentic-harness-engineering

---
_자동 Wiki Query에서 추출됨_
