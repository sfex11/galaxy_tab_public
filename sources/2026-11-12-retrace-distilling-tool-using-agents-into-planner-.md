# ReTrace: Distilling Tool-Using Agents into Planner-Free Workflows

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-12
**링크**: http://arxiv.org/abs/2611.14492v1

## 💡 핵심 인사이트

반복 SOP 실행에서 에이전트의 매단계 LLM 추론은 불필요한 유연성 비용이므로, 실행 로그와 그 추론 텍스트를 코드 워크플로우로 컴파일하면 정책이 모델에서 코드로 이주한다.

## 📖 분석

ReTrace는 반복 SOP 실행에서 LLM이 매 단계 선택을 수행하는 비용·지연 문제를, SOP 자연어 명세와 소수의 로깅된 에이전트 실행을 재사용 가능한 워크플로우로 컴파일하여 해소한다. 산출물에서는 코드가 다음 단계를 선택하고 단계별 LLM 호출이 사라진다.

이 논문의 위키 내 위치는 세 축에서 규정된다. 첫째, harness-as-nonparametric-policy-layer의 완성형 실현이다 — 실행 로그라는 태스크 피드백으로부터 '접근→결정' 정책을 코드 워크플로우라는 비파라메트릭 계층으로 학습한다. 둘째, demonstration-to-code-compilation의 원천 교체다 — RAPID 계열의 시각 시연이 아니라 에이전트 실행 로그가 컴파일 소스가 되며, 각 도구 호출에 에이전트가 작성한 설명(추론 텍스트)이 분기 조건 학습의 원료로 재활용된다. 셋째, harness-distillation의 방향 반전이다 — 하네스 기능의 모델 내면화(runtime-to-parametric-memory-absorption)와 정반대로, 모델의 런타임 정책을 코드로 외재화하여 agentic-distillation(모델 소형화)과 질적으로 다른 비용 절감 경로를 연다.

SOP 명세가 판단 클래스를 배포 전에 확정한다는 점에서 compilation-as-offline-commitment의 적용 사례이며, 반복 실행에서 에이전트 루프의 계산을 정적 코드로 대체함으로써 agent-loop-as-computation 관점의 경제적 하한을 낮춘다. 유연성이 불필요한 반복 프로세스에서 에이전시의 위상이 '실행 주체'에서 '컴파일 원천'으로 이동함을 보여준다.

## 🔗 관련 논문

- ReTrace: Distilling Tool-Using Agents into Planner-Free Workflows

## 🏷️ 엔티티

- [[entities/agent-to-workflow-compilation.md|agent-to-workflow-compilation]]
- [[entities/harness-as-nonparametric-policy-layer.md|harness-as-nonparametric-policy-layer]]
- [[entities/demonstration-to-code-compilation.md|demonstration-to-code-compilation]]
- [[entities/harness-distillation.md|harness-distillation]]
- [[entities/compilation-as-offline-commitment.md|compilation-as-offline-commitment]]
- [[entities/execution-record-as-learning-corpus.md|execution-record-as-learning-corpus]]
- [[entities/agent-loop-as-computation.md|agent-loop-as-computation]]

## 📐 개념

- [[concepts/agent-to-workflow-compilation.md|agent-to-workflow-compilation]]
- [[concepts/reasoning-as-compilation-source.md|reasoning-as-compilation-source]]

---
_LLM 분석으로 생성됨_
