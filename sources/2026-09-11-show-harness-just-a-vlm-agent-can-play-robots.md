# Show-Harness: Just a VLM Agent Can Play Robots

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10522v1

## 💡 핵심 인사이트

세계 지능에서 로봇 제어로의 병목은 모델 능력이 아니라 의도-행동 인터페이스 설계이며, 동결된 VLM에 이산적 의미 행동 단위와 결정론적 인터프리터만 제공하면 로봇을 '플레이'할 수 있다.

## 📖 분석

Show-Harness는 범용 VLM을 그대로 두고('just a VLM agent') 로봇 조작을 가능하게 하는 Embodied Harness를 제안한다. 핵심은 의도(intent)와 행동(action)을 연결하는 컴팩트한 의미 인터페이스다. VLM은 이산적 의미 행동 단위(semantic action unit)를 추론하고, 구현(embodiment) 특유의 인터프리터가 이를 국소 로봇 행동으로 결정론적으로 grounding한다. 세계 지능을 담당하는 VLM과 운동 제어를 담당하는 하네스의 책임이 명시적으로 분리된다.

Wiki 관점에서 이 논문은 세 축을 강화한다. 첫째, representation-action-gap의 제3 해법 경로: Continuous Actions from Discrete Minds([[latent-aligned-planning]])가 잠재 공간 정렬로 간극을 봉합했다면, 본 논문은 모델을 수정하지 않고 표현 계약을 인터페이스 계층으로 외면화한다. 둘째, harness-side-compensation의 체화 확장: SENTINEL-RL이 위상 추론을 하네스로 오프로딩했다면, 본 논문은 운동 제어 전체를 인터프리터로 오프로딩하여 하네스가 추론의 구성요소임을 강화한다. 셋째, end-to-end VLA 훈련([[vla-foundry]])과 대비되는 '동결 모델 + 인터페이스 설계' 전략으로 체화 능력 확보 스펙트럼에 훈련-무관 축을 추가한다. 결정론적 인터프리터는 실행 검증 대상을 모델 출력에서 인터페이스 계약 준수로 구체화한다.

## 🔗 관련 논문

- Continuous Actions from Discrete Minds: Latent-Aligned Planning for En
- VLA Foundry: A Unified Framework for Training Vision-Languag
- SENTINEL-RL: Offloading Topological Reasoning from LLM Agent
- Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Mo
- Towards Trustworthy Autonomous Robots: An Explainable AI-Bas

## 🏷️ 엔티티

- [[entities/show-harness.md|show-harness]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/representation-action-gap.md|representation-action-gap]]
- [[entities/action-tokenization.md|action-tokenization]]
- [[entities/latent-aligned-planning.md|latent-aligned-planning]]
- [[entities/harness-side-compensation.md|harness-side-compensation]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/vla-foundry.md|vla-foundry]]
- [[entities/representation-contract.md|representation-contract]]
- [[entities/execution-verification.md|execution-verification]]

## 📐 개념

- [[concepts/semantic-action-unit.md|semantic-action-unit]]
- [[concepts/embodied-harness.md|embodied-harness]]
- [[concepts/embodiment-specific-interpreter.md|embodiment-specific-interpreter]]
- [[concepts/deterministic-grounding.md|deterministic-grounding]]
- [[concepts/intent-action-interface.md|intent-action-interface]]

---
_LLM 분석으로 생성됨_
