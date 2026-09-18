# In-Context Robot Learning with VLM Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-18
**링크**: http://arxiv.org/abs/2609.19138v1

## 💡 핵심 인사이트

일반화의 병목이 유한한 데모 커버리지에 있을 때 해법은 데모를 가중치에 컴파일하는 것이 아니라 배포 시점 컨텍스트로 소비하는 것이며, 이는 VLM 에이전트의 ICL 능력이 물리 세계로 이전 가능함을 전제로 한다.

## 📖 분석

# In-Context Robot Learning with VLM Agents (2026-09-18)

## 핵심 주장
로봇이 낯선 환경에 인간처럼 적응하려면 배포 시점에 컨텍스트로부터 학습하는 능력(ICL)이 필수적이다. 유한한 데모 수집은 로봇이 마주칠 모든 태스크와 상황을 커버할 수 없으므로, 일반화의 조건은 데모의 양이 아니라 데모의 소비 방식에 있다. 본 논문은 상용 VLM(GPT-6 Astra)의 에이전틱 능력을 활용해 기존 로봇 정책의 도달 밖이던 ICL을 실현한다.

## Wiki에서의 위치
[[in-context-learning]] 개념에 로봇 도메인 착상을 제공하는 사례다. 데모를 훈련 데이터(가중치 흡수)가 아닌 배포 시점 컨텍스트(추론 조건화)로 소비하는 재프레이밍은 [[marginal-distribution-ceiling]]의 커버리지 천장을 우회하는 경로다. [[show-harness]]가 VLM 에이전트가 로봇을 '플레이'함을 보였다면, 본 논문은 같은 에이전트가 컨텍스트로 '학습'까지 수행함으로 확장한다. [[vla-foundry]] 계열의 미세조정 중심 VLA 패러다임과 대비되는 훈련 프리 적응 축을 열며, 궤적의 스킬·환경·코칭 소비([[experience-reuse]])에 이어 'ICL 컨텍스트'라는 제4 소비 경로를 추가한다. 또한 [[frozen-model-external-memory-contradiction]]에서 진단된 동결 모델-동적 환경 간극이 외부 메모리가 아닌 컨텍스트 자체로 봉합될 수 있음을 보여준다.

## 핵심 통찰
일반화의 병목이 데모 커버리지에 있을 때, 해법은 데모를 파라미터에 컴파일하는 것이 아니라 배포 시점 컨텍스트로 두는 것이다.

## 🔗 관련 논문

- Show-Harness: Just a VLM Agent Can Play Robots
- VLA Foundry: A Unified Framework for Training Vision-Languag
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En

## 🏷️ 엔티티

- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/agentic-vlm.md|agentic-vlm]]
- [[entities/show-harness.md|show-harness]]
- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/frozen-model-external-memory-contradiction.md|frozen-model-external-memory-contradiction]]

## 📐 개념

- [[concepts/in-context-learning.md|in-context-learning]]
- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/generalization-gap.md|generalization-gap]]
- [[concepts/experience-reuse.md|experience-reuse]]
- [[concepts/demonstration-as-context.md|demonstration-as-context]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-17-where-should-a-document-live-context-representatio]]: 지식을 가중치에 컴파일하는 대신 배포 시점에 컨텍스트로 소비하는 것이 효율적·유연한 적응 경로라는 공통 전제를 공유한다.
- → [[sources/2026-09-18-cognitive-extensions-for-dual-process-language-age]]: 재훈련 없이 배포 시점 컨텍스트 소비(ICL)와 부착형 기억 모듈(AMM)로 적응을 달성한다는 '컴파일이 아닌 소비·부착' 전략을 공유한다.
