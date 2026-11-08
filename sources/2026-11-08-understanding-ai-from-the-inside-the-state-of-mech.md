# Understanding AI from the Inside: The State of Mechanistic Interpretability for AI Safety

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08438v1

## 💡 핵심 인사이트

기계론적 해석가능성은 '이해하지 못하는 시스템을 계속 구축한다'는 안전-이해 간극을 닫는 유일하게 체계적 경로이며, 해석 감사가 가리키는 내부 실재의 반증 가능성이라는 접지 특권이 그 신뢰성의 1차 담보다.

## 📖 분석

기계론적 해석가능성 연구를 AI 안전 관점에서 종합하는 서베이다. 신경망이 인류 역사상 가장 중요한 인공물이 될 가능성이 높은데도 작동 원리·미지 상황 행동·제어 방법을 모른 채 구축이 가속되는 안전-이해 간극([[concepts/safety-understanding-gap.md|safety understanding gap]])을 문제 설정으로 삼는다.

Wiki의 해석가능성 축과의 정합성: Legibility is Not Interpretability가 실증한 '가독성≠해석가능성'([[concepts/legibility-interpretability-gap.md|legibility interpretability gap]])과 MoRFI의 인과적 개입 검증 흐름을 서베이 차원에서 체계화하여, [[concepts/causal-mechanistic-interpretability.md|causal mechanistic interpretability]]를 표준 방법론으로 규정한다.

세 가지 핵심 기여: (1) 해석 감사의 접지 특권([[concepts/interpretability-grounding-privilege.md|interpretability grounding privilege]]) — 검증 대상이 실재하며 activation patching으로 반증 가능하다는 타 도메인에 없는 특권. (2) 해석-제어 파이프라인([[concepts/interpretability-control-pipeline.md|interpretability control pipeline]]) — 판독→인과 검증→개입→제어의 연쇄로, Deep Noir가 실증한 read-to-manipulate 경로([[concepts/steering-read-manipulation-duality.md|steering read manipulation duality]])를 일반 원리로 격상. (3) 인간 용량 병목 — 해석 연구의 확장 문제의식이 SAEScientist-Bench 계열 자동화 연구([[entities/autonomous-interpretability-research.md|autonomous interpretability research]])의 근거가 되되, 감사 자율화는 재귀적 감사 문제를 수반함을 제기한다.

기존 Wiki가 흩어져 축적한 해석 감사·스티어링·CoT 감시 연구를 '이해가 제어의 전제'라는 단일 파이프라인으로 묶는 종합적 위상 정리다.

## 🔗 관련 논문

- SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Interp
- Legibility is Not Interpretability: Comparing Judged and Actual Import
- MoRFI: Monotonic Sparse Autoencoder Feature Identification
- Deep Noir: Autonomous Steering Discovery via Architectural Chronometry
- User Model Extraction via Belief Self-Distillation
- Corrupt Plans, Clean Traces: Evading Chain-of-Thought Monito

## 🏷️ 엔티티

- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/interpretability-grounding-privilege.md|interpretability-grounding-privilege]]
- [[entities/safety-understanding-gap.md|safety-understanding-gap]]
- [[entities/interpretability-control-pipeline.md|interpretability-control-pipeline]]
- [[entities/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[entities/autonomous-interpretability-research.md|autonomous-interpretability-research]]
- [[entities/saescientist-bench.md|saescientist-bench]]
- [[entities/activation-patching.md|activation-patching]]
- [[entities/steering-read-manipulation-duality.md|steering-read-manipulation-duality]]
- [[entities/sparse-autoencoder.md|sparse-autoencoder]]

## 📐 개념

- [[concepts/legibility-interpretability-gap.md|legibility-interpretability-gap]]
- [[concepts/read-to-manipulate-pipeline.md|read-to-manipulate-pipeline]]
- [[concepts/interpretability-as-audit-layer.md|interpretability-as-audit-layer]]
- [[concepts/causal-load-verification.md|causal-load-verification]]
- [[concepts/safety-understanding-gap.md|safety-understanding-gap]]

---
_LLM 분석으로 생성됨_
