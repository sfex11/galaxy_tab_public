# AgentSSL: Can MLE Agents Leverage Unlabeled Data?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-14
**링크**: http://arxiv.org/abs/2611.17323v1

## 💡 핵심 인사이트

MLE 에이전트의 실용 병목이 파이프라인 설계 자동화에서 레이블 부재 하의 학습 신호 구성으로 이동하며, SSL을 프로그램 탐색으로 재프레이밍하면 에이전트의 탐색 능력이 학습 절차 자체의 발견으로 확장된다.

## 📖 분석

AgentSSL은 MLE 에이전트 연구가 완전 지도 학습 설정에만 국한되어 온 간극을 진단하고, 레이블이 희소하고 레이블 없는 데이터가 풍부한 현실적 체제에서 에이전트가 파이프라인을 자동 설계할 수 있는지를 문제화한다. 핵심 기여는 SSL을 프로그램 탐색 문제로 재프레이밍하는 것이다 — 에이전트가 레이블 없는 데이터에서 유의미한 학습 절차(프로그램)를 탐색·발견한다는 구조. 이는 [[agent-to-workflow-compilation]]과 동형이다. ReTrace(sources/2026-11-12-retrace-distilling-tool-using-agents-into-planner-free-workflows)가 실행 로그에서 워크플로우를 컴파일했다면, AgentSSL은 언레이블 데이터에서 SSL 전략을 컴파일한다. 컴파일 대상이 행동 시퀀스에서 학습 절차로 이동하는 새 축을 형성한다.

[[self-training-data-construction]] 계보의 확장이기도 하다. Strategically Diverse Sampling(sources/2026-09-29-strategically-diverse-sampling-for-self-training)이 샘플 생성 전략을, GEPA-Curator(sources/2026-10-29-gepa-curator-curated-learning-for-self-improving-agents)가 태스크 큐레이션을 다뤘다면, AgentSSL은 레이블 부재 조건에서 데이터 자체의 가치 추출을 다룬다. [[environment-capability-causality]] 관점에서 데이터 가용성 구조(희소 레이블+풍부 언레이블)가 에이전트 능력 발현의 상한과 방향을 결정하는 새 조건이 된다. [[autoresearch]]의 실용화 경로도 제시한다 — 완전 지도 학습 전제의 자동화가 실제 배포 제약(레이블 획득 비용)을 만나는 지점을 규정한다.

## 🔗 관련 논문

- retrace-distilling-tool-using-agents-into-planner-free-workflows
- strategically-diverse-sampling-for-self-training
- gepa-curator-curated-learning-for-self-improving-agents

## 🏷️ 엔티티

- [[entities/agentssl.md|agentssl]]

## 📐 개념

- [[concepts/ssl-as-program-search.md|ssl-as-program-search]]
- [[concepts/label-scarcity-regime.md|label-scarcity-regime]]
- [[concepts/supervised-only-mle-agent-assumption.md|supervised-only-mle-agent-assumption]]

---
_LLM 분석으로 생성됨_
