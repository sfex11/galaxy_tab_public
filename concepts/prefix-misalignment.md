# 접두사 불일치

**생성일**: 2026-06-17

## 정의

토큰 압축/제거 시 중간 토큰이 빠지면 KV 캐시의 위치 기반 인덱싱이 깨져 이후 모든 토큰의 캐시 라인이 물리적으로 불일치하는 현상으로, 논리적 압축의 정답이 하드웨어 캐시의 오답이 되는 지점이다.

## 관련 논문

- kv-cache-optimization
- algorithm-system-translation-gap

---
_자동 Wiki Query에서 추출됨_
