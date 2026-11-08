# VeriCUA: Verification as Agentic Exploration for Computer-Using Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-02
**링크**: http://arxiv.org/abs/2610.40578v1

## 💡 핵심 인사이트

CUA 검증의 병목은 판정 능력이 아니라 증거 수집 능력이며, 검증자가 환경을 직접 탐색해야만 VLM judge와 생성 프로그램 모두의 부분 관측 사각지대가 해소된다.

## 📖 분석

## VeriCUA: 검증 = 에이전틱 탐색 (v1 정식 등록)

CUA(컴퓨터 사용 에이전트)의 스케일링은 데이터 큐레이션·평가·RL을 위한 신뢰할 수 있는 태스크 완수 검증을 요구한다. 기존 자동 검증은 두 경로로 갈렸다: VLM judge(제공된 관측에만 의존)와 생성 프로그램(접근 가능한 상태에만 의존). 본 논문은 양쪽 모두 partial-view-verification-limitation에 갇혀 있음을 진단하고, 검증 자체를 에이전틱 탐색으로 재정의한다 — 검증자가 환경을 능동적으로 탐색하여 증거를 수집한 뒤 판정한다.

이는 [[concepts/verification-as-agentic-exploration.md|verification as agentic exploration]]의 원천 정의를 확정하며, [[concepts/verifier-as-agent.md|verifier as agent]]의 구체적 구현이다. 검증의 병목이 판정 능력이 아니라 증거 수집 능력에 있다는 발견은 [[concepts/access-planning-gap.md|access planning gap]]의 검증 도메인 버전이다.

관점적으로 이는 [[concepts/environment-grounded-validity.md|environment grounded validity]]의 CUA 실현이자 [[concepts/execution-verification.md|execution verification]]의 강화다. 다만 탐색이 VLM 능력에 의존하므로 완전한 non-cognitive-oracle은 아니며, '탐색 매개 검증'이라는 중간 지점을 보여준다. [[concepts/independent-success-adjudication.md|independent success adjudication]] 관점에서 성공 판정의 상한이 검증자의 탐색 능력에 의해 결정됨이 새 조건으로 추가된다. [[concepts/computer-use-agent.md|computer use agent]] 생태계의 검증 인프라 병목 해소 경로를 제공한다.

## 🔗 관련 논문

- VeriCUA: Verification as Agentic Exploration for Computer-Using Agents

## 🏷️ 엔티티

- [[entities/vericua.md|vericua]]
- [[entities/verification-as-agentic-exploration.md|verification-as-agentic-exploration]]
- [[entities/verifier-as-agent.md|verifier-as-agent]]
- [[entities/partial-view-verification-limitation.md|partial-view-verification-limitation]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/environment-grounded-validity.md|environment-grounded-validity]]
- [[entities/non-cognitive-oracle.md|non-cognitive-oracle]]
- [[entities/independent-success-adjudication.md|independent-success-adjudication]]

## 📐 개념

- [[concepts/verification-as-agentic-exploration.md|verification-as-agentic-exploration]]
- [[concepts/partial-view-verification-limitation.md|partial-view-verification-limitation]]
- [[concepts/verifier-as-agent.md|verifier-as-agent]]
- [[concepts/environment-grounded-validity.md|environment-grounded-validity]]
- [[concepts/non-cognitive-oracle.md|non-cognitive-oracle]]
- [[concepts/independent-success-adjudication.md|independent-success-adjudication]]

---
_LLM 분석으로 생성됨_
