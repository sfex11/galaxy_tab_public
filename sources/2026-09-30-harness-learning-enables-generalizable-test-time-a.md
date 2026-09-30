# Harness Learning Enables Generalizable Test-Time Adaptation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35738v1

## 💡 핵심 인사이트

에이전트의 적응 표면은 모델 가중치만이 아니라 하네스라는 실행 프로그램이며, 실행 피드백으로 하네스를 개정하는 프로포저를 훈련하면 테스트타임 적응이 파라미터 업데이트 없이 프로그램 위의 메타학습으로 일반화 가능하게 실현된다.

## 📖 분석

# Harness Learning Enables Generalizable Test-Time Adaptation

에이전트는 모델과 하네스(모델 호출·도구 사용·정보 흐름을 조직하는 실행 프로그램)의 결합체다. 본 논문은 프로포저 모델이 실행 피드백으로 솔버의 하네스를 개정하도록 훈련하는 **하네스 학습**을 도입하고, 이를 실행 가능 프로그램 위의 [[meta-learning]]으로 형식화한다.

Wiki의 하네스 계열 연구는 3단계로 축적되어 왔다: 하네스 설계 선택이 성능을 좌우함을 실증한 진단 단계([[harness-engineering]], [[agentic-harness-engineering]]), 실패 피드백으로 하네스를 성장시킨 휴리스틱 단계([[growing-harness]], [[failure-guided-harness-growth]]), 하네스-모델 결합 최적화 단계([[harness-model-co-evolution]]). 본 논문은 제4단계를 연다 — 하네스 개정 정책 자체를 학습하는 단계다.

핵심은 테스트타임 적응의 매체 전환이다. 추론 컴퓨트 확장([[test-time-scaling]])이나 가중치 훈련이 아닌 제어 계층 프로그램의 개정으로 적응이 일어난다. 솔버를 동결한 채 하네스만 개정하므로 능력 번역자([[harness-as-capability-translator]])가 학습 대상이 되며, 파라미터 업데이트 없는 적응([[retraining-free-adaptation]])의 하네스 버전을 제공한다. 프로포저-솔버 분리는 문제 출제자-해결자 분리([[solver-poser-decoupling]])의 시스템 자기개정 확장이기도 하다.

## 🔗 관련 논문

- Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Intelligence
- Agentic Harness Engineering: Observability-Driven Automatic Evolution
- Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Models
- SafeEvolve: Harness-Policy Co-Evolution from Agent Experience
- An Empirical Study of Harness Design for Coding Agents
- Efficient Test-Time Adaptation through Human-AI Interaction

## 🏷️ 엔티티

- [[entities/harness-learning.md|harness-learning]]
- [[entities/agentic-harness-engineering.md|agentic-harness-engineering]]
- [[entities/harness-model-co-evolution.md|harness-model-co-evolution]]
- [[entities/growing-harness.md|growing-harness]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/harness-as-capability-translator.md|harness-as-capability-translator]]
- [[entities/retraining-free-adaptation.md|retraining-free-adaptation]]

## 📐 개념

- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/failure-guided-harness-growth.md|failure-guided-harness-growth]]
- [[concepts/control-semantic-division.md|control-semantic-division]]
- [[concepts/test-time-compute-harness-mapping.md|test-time-compute-harness-mapping]]
- [[concepts/solver-poser-decoupling.md|solver-poser-decoupling]]

---
_LLM 분석으로 생성됨_
