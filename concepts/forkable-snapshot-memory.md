# 포크 가능 스냅샷 메모리

**생성일**: 2026-11-03

## 정의

KV 캐시의 불변 접두사+append 방식 prefix 공유를 대체하여, 값 의미론(value semantics)의 전체 복사가 가능한 불변 스냅샷과 delta로 상태를 관리하는 메모리·캐시 계층 설계.

## 관련 논문

- kv-cache-optimization
- agent-sandbox-state-management
- exact-state-forking
- attention-carried-conversational-state

---
_자동 Wiki Query에서 추출됨_
