# TAMPAgent: Agentic Belief-Space Planning for Mobile Manipulation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-04
**링크**: http://arxiv.org/abs/2611.03584v1

## 💡 핵심 인사이트

LVLM의 개방형 추론과 TAMP의 기하학적 건전성은 대체재가 아니라 위임 관계로 결합될 수 있다 — 부분 관측 하 신념 공간 계획은 LVLM이 수행하고 고비용 기하 탐색은 TAMP에 위임함으로써 두 패러다임의 상보적 약점이 동시에 해소된다.

## 📖 분석

TAMPAgent는 LVLM 에이전트의 개방형 추론과 TAMP의 기하학적 건전성을 결합한 모바일 매니퓰레이션 아키텍처를 제시한다. 핵심 진단은 두 패러다임의 상보적 약점이다: 직접 도구 호출 방식의 agentic-vlm는 기하학적 불확실성을 처리하지 못해 완전 관측 테이블톱 환경에 갇혔고, TAMP는 부분 관측 하 장기 과제를 풀 수 있으나 계산 비용이 과도하다.

Wiki 논의에 대한 두 가지 기여가 있다. 첫째, [[concepts/belief-state-grounding.md|belief state grounding]] 계열의 신념 개념을 '검색 질의의 조건'에서 '계획의 작업 공간'으로 격상한다 — 부분 관측 하에서 LVLM이 신념 상태를 유지·갱신하며 그 위에서 행동을 선택하는 신념 공간 계획(belief-space planning)이 물리 도메인에서 실현된다. 둘째, [[concepts/generalized-tamp.md|generalized tamp]]가 보여준 '코딩 에이전트가 TAMP 도메인 코드를 저작'과 대비되는 새 결합 방향, 즉 LVLM이 TAMP 솔버를 고비용 기하 탐색의 위임 백엔드로 사용하는 방식을 제시한다. 이는 [[concepts/latent-aligned-planning.md|latent aligned planning]]의 공유 잠재 정렬과 대비되는, 표현 정렬이 아닌 역할 분할로 [[concepts/thinking-acting-gap.md|thinking acting gap]]을 봉합하는 제2의 경로다. [[concepts/planning-without-physical-constraint-encoding.md|planning without physical constraint encoding]]의 진단에 '제약 인코딩된 솔버 위임'이라는 구조적 해법을 공급하며, [[concepts/access-planning-gap.md|access planning gap]]의 역방향 문제(계산 능력은 있으나 정보가 부분적)를 다룬다. [[concepts/dual-process-agent.md|dual process agent]]에는 '느린 체계적 탐색(TAMP)을 위임 대상으로 삼는' 물리 도메인 실현을 추가한다.

## 🔗 관련 논문

- Coding Agents for Generalized Task and Motion Planning Problems
- RunAgent: Interpreting Natural-Language Plans with Constraint-Guided Execution
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for End-to-End Driving
- Jev-Mobile: Jev as an Executor for Mobile GUI Agents
- TANDEM: Task and Motion Planning with As-Needed Demonstration
- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation

## 🏷️ 엔티티

- [[entities/belief-space-planning.md|belief-space-planning]]
- [[entities/geometric-search-delegation.md|geometric-search-delegation]]
- [[entities/generalized-tamp.md|generalized-tamp]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/dual-process-agent.md|dual-process-agent]]

## 📐 개념

- [[concepts/thinking-acting-gap.md|thinking-acting-gap]]
- [[concepts/latent-aligned-planning.md|latent-aligned-planning]]
- [[concepts/access-planning-gap.md|access-planning-gap]]
- [[concepts/planning-without-physical-constraint-encoding.md|planning-without-physical-constraint-encoding]]
- [[concepts/belief-state-grounding.md|belief-state-grounding]]
- [[concepts/imperfect-perception.md|imperfect-perception]]
- [[concepts/harness-methodology-embodiment-migration.md|harness-methodology-embodiment-migration]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-11-06-vabar-a-variational-automation-benchmark-for-agent]]: LVLM+TAMP 결합이 겨냥하는 부분 관측 하 agentic 로봇 조작 과제를 VABAR가 변동 자동화라는 벤치마크 틀로 형식화하여 평가 지점을 제공한다.
