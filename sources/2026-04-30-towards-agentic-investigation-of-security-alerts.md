# Towards Agentic Investigation of Security Alerts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25846v1

## 💡 핵심 인사이트

보안 조사와 같은 고신뢰 도메인에서는 에이전트의 도구 공간을 설계 시점에 구조적으로 제약하는 정적 접근이, 런타임에 동적으로 도구를 게이팅하는 접근보다 검증 가능성 측면에서 실무적으로 우월할 수 있음을 보여준다.

## 📖 분석

# Towards Agentic Investigation of Security Alerts

**카테고리**: AI/ML — 보안 자동화
**생성일**: 2026-04-30

## 정의

보안 경보(Security Alert)의 초기 조사 단계를 자동화하기 위해, LLM 에이전트에 사전 정의된 쿼리와 제약된 도구 접근(Suricata 로그에 대한 구조화 SQL, grep 기반 텍스트 검색)을 결합한 실험적 에이전틱 워크플로우.

## 기존 Wiki와의 관계

이 논문은 Wiki에서 논의된 **제어된 자율성(controlled-autonomy)** 원칙의 구체적 실현 사례다. 개방형 도구 사용(computer-use-agent)이 아닌, 도메인 특화된 제약 도구 집합만 에이전트에 부여함으로써 신뢰성과 범용성 사이의 트레이드오프를 실무적으로 해결한다. 이는 [[entities/tool-attention|tool-attention]]의 동적 게이팅 접근과 상보적 위치에 있다: tool-attention이 런타임에 도구를 선택적으로 노출한다면, 본 논문은 설계 시점에 도구 공간을 사전 제약한다.

[[entities/zero-trust-agent-architecture|zero-trust-agent-architecture]]의 제약 원칙을 보안 운영(SecOps) 도메인에 적용한 구체적 인스턴스이기도 하다. 에이전트가 임의의 시스템 명령을 실행할 수 없고, 사전 정의된 SQL 쿼리와 grep 패턴만 사용 가능하도록 구조적으로 격리한다는 점에서 [[concepts/structural-isolation|구조적 격리]] 패턴을 따른다.

## 핵심 설계 선택

- **제약된 도구 접근**: 개방형 컴퓨터 사용이 아닌 구조화된 쿼리만 허용
- **사전 정의된 쿼리**: Suricata 로그 스키마에 맞춘 SQL 템플릿 기반
- **다중 로그 소스 상관관계**: 수동 상관관계 작업을 에이전트가 자동 수행

## 연결점

- [[sources/2026-04-23-an-ai-agent-execution-environment-to-safeguard-use.md|실행 환경 기반 사용자 데이터 보호]]와 대비: 해당 논문이 데이터 접근을 구조적 격리로 제한한다면, 본 논문은 도구 접근을 구조적 격리로 제한한다.
- [[sources/2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md|Tool Attention]]과의 차이: 동적 게이팅 vs. 정적 제약이라는 상보적 접근

## 🔗 관련 논문

- 2026-04-23-an-ai-agent-execution-environment-to-safeguard-use.md
- 2026-04-25-tool-attention-is-all-you-need-dynamic-tool-gating.md

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/tool-attention.md|tool-attention]]
- [[entities/zero-trust-agent-architecture.md|zero-trust-agent-architecture]]
- [[entities/agentic-security-investigation.md|agentic-security-investigation]]

## 📐 개념

- [[concepts/constrained-tool-access.md|constrained-tool-access]]
- [[concepts/alert-triage-automation.md|alert-triage-automation]]
- [[concepts/structured-query-augmented-agent.md|structured-query-augmented-agent]]
- [[concepts/security-operations-agent.md|security-operations-agent]]

---
_LLM 분석으로 생성됨_
