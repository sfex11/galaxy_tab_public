# Context-Assemble Bridge Pattern (컨텍스트 어셈블 브리지)

**분야**: Agent Architecture / Integration Pattern
**생성일**: 2026-04-17

## 정의

외부 컨텍스트 관리 도구(예: opencode-contexty)를 에이전트 프레임워크(예: OpenClaw)에 통합할 때, 직접 포팅 대신 **외부 context builder + 프레임워크 skill 주입** 방식으로 연결하는 패턴.

## 핵심 구조

```
메시지 수신 → Context Builder (외부) → context file 생성 → 에이전트가 read로 읽음 → 작업 수행
```

## 장점

- **변경에 강함**: 프레임워크 업스트림이 바뀌어도 브리지만 수정
- **격리**: 컨텍스트 생성과 에이전트 실행 분리
- **재사용**: Context Builder를 다른 프레임워크에서도 사용 가능

## 구현 요건

1. 산출물 분류: "항상 필요한 것" vs "질문마다 바뀌는 것"
2. 상시 규칙 → 프레임워크 워크스페이스 파일로 변환
3. 동적 문맥 → 별도 스크립트로 생성 → 임시 파일에 저장
4. 세션별 격리 유지 (session_id 기준)

## Wiki 연결

이 패턴은 [[concepts/dynamic-context-injection|동적 컨텍스트 주입]]의 구현 전략이며, [[concepts/epistemic-infrastructure|인식론적 인프라]]의 동기화 계층(Synchronization Layer)과 유사한 역할.

---
_OpenClaw + opencode-contexty 적용 분석에서 추출됨 (2026-04-17)_
