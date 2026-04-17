# Dynamic Context Injection (동적 컨텍스트 주입)

**분야**: Agent Architecture / Context Management
**생성일**: 2026-04-17

## 정의

에이전트가 작업을 수행할 때, 프로젝트 규칙·문서·메모리 등 필요한 문맥을 자동으로 수집해 LLM 입력에 주입하는 기법. 정적(항상 필요)과 동적(질문마다 변함) 컨텍스트를 분리 관리.

## 3단계 아키텍처

1. **Indexer** — 프로젝트 문서, 코드 규칙, ADR, 이슈 메모를 수집해 구조화
2. **Selector** — 현재 메시지/작업 목표를 보고 관련 컨텍스트만 선택 (랭킹 + 절삭)
3. **Injector** — 선택된 결과를 에이전트 세션의 프롬프트에 주입

## 컨텍스트 분류

| 유형 | 예시 | 주입 위치 |
|------|------|----------|
| **고정 규칙** | 코딩 스타일, 레포 구조, 금지사항 | AGENTS.md |
| **도메인 지식** | API 설명, 아키텍처, 운영 절차 | skills/*/SKILL.md |
| **동적 문맥** | 현재 이슈, 최근 변경, 관련 함수 | .runtime/context/current-task.md |

## 주의점

- **토큰 낭비 방지**: 원문 통째로 주입 금지. "정책 10줄 + 관련 파일 5개 + 요약 20줄"처럼 압축
- **세션 격리**: session_id/agent_id 기준으로 캐시 분리 → 문맥 오염 방지
- **워크스페이스 범위 제한**: 외부 파일시스템 전체 읽기는 보안 위험

## 관련 프로젝트

- [opencode-contexty](https://github.com/ttalkkak-lab/opencode-contexty) — OpenCode용 컨텍스트 관리 도구

## Wiki 연결

이 개념은 에이전트의 인식론적 인프라(epistemic infrastructure)의 **실제 구현 패턴**으로 이해할 수 있음. 지식을 구조화하고 선택적으로 주입하는 것은 4계층 인식론적 인프라의 기술적 구현.

→ [[concepts/epistemic-infrastructure|인식론적 인프라]]
→ [[concepts/agent-identity|에이전트 아이덴티티]] (컨텍스트 = 정체성의 기술적 차원)

---
_OpenClaw + opencode-contexty 적용 분석에서 추출됨 (2026-04-17)_
