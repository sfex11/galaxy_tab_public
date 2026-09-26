# 추적 쓰기 주체 분리

**생성일**: 2026-09-26

## 정의

에이전트의 도구 호출은 추적의 작성자(author)가 아니라 하네스 소유 기록기의 입력이 되어야 한다는 설계 원칙. 계산의 실행 기록은 계산되는 프로그램이 아니라 런타임의 소유물임을 원칙화하여, 추적 무결성을 에이전트 쓰기 권한으로부터 구조적으로 분리한다.

## 관련 논문

- agent-as-harness
- agent-loop-as-computation
- append-only-trace-enforcement
- agentic-harness-engineering

---
_자동 Wiki Query에서 추출됨_
