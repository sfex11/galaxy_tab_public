# When LLM Decompilers Recompile More and Preserve Less

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05370v1

## 💡 핵심 인사이트

LLM 디컴파일러의 재컴파일 가능성은 유창한 코드라는 실패의 은폐를 인증할 뿐 원본 소스의 정보 보존과 무관하며, 이는 '표면 신호 통과 ≠ 실제 목표 달성'이라는 평가 계약 결함의 리버스 엔지니어링 발현이다.

## 📖 분석

# When LLM Decompilers Recompile More and Preserve Less (2026-09-08)

## 핵심 발견

LLM 기반 디컴파일러는 Ghidra·Hex-Rays 같은 전통적 도구와 달리 깔끔하고 컴파일 가능한 C 코드를 생성하지만, 이 유창함이 원본 소스의 정보 보존과 무관함을 실증한다. '재컴파일 가능성·재실행 가능성'이라는 현재 표준 평가 기준은 [[meaning-insensitive-metric]]의 리버스 엔지니어링 발현이다 — WER이 음성의 의미를, 코드 커버리지가 기능적 검증 적합성을 측정하지 못하듯, 재컴파일 성공은 기계 코드의 의미 보존을 측정하지 못한다.

## Wiki 지형에서의 위치

2026년 9월 평가 계약 비판의 흐름에 세 번째 축을 추가한다:
- [[swe-gate]]: 테스트 통과 ≠ 패치 수용
- [[legibility-interpretability-gap]]: 가독성 ≠ 기능적 역할
- 본 논문: 재컴파일 가능 ≠ 정보 보존

셋 모두 [[single-surface-signal-insufficiency]] — 단일 표면 신호가 실제 목표를 대체할 수 없다는 원칙의 도메인 발현이며, [[coverage-functionality-gap]]이 평가 방법론의 범용적 결함임을 강화한다.

## 새로운 인사이트: 실패 가시성의 역전

가장 독특한 기여는 [[ontological-concealment-of-failure]]의 대비 구조다. 전통적 디컴파일러는 해결 못한 부분을 플레이스홀더로 드러내어 — 불완전하지만 — 정직하다. LLM 디컴파일러는 유창한 코드로 소실된 정보의 부재조차 은폐한다. 이는 [[cot-as-translated-report]]의 확장이다: 디컴파일 출력은 기계 코드의 '번역된 보고서'이며, 가독성이 계산의 실재를 전달한다는 보장이 없다. 평가 지표가 이 은폐를 감지하지 못하면 [[fidelity-illusion]]이 완성된다 — 빌드·테스트 통과라는 [[execution-verification]]의 성공 신호가 실제로는 정보 손실의 인증서로 기능한다. [[surface-completeness-misreading]]과 [[binary-analysis]] 도메인의 연결점도 제공한다.

## 🔗 관련 논문

- SWE-Gate: Passing Functional Tests Is Not Enough for Softwar
- Legibility is Not Interpretability: Comparing Judged and Act
- RESTestBench: A Benchmark for Evaluating the Effectiveness o
- Evaluation of Automatic Speech Recognition Using Generative
- Clean Engineering, Unstable Measurement: A Preregistered Rel

## 🏷️ 엔티티

- [[entities/llm-decompiler.md|llm-decompiler]]
- [[entities/binary-analysis.md|binary-analysis]]
- [[entities/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[entities/coverage-functionality-gap.md|coverage-functionality-gap]]
- [[entities/ontological-concealment-of-failure.md|ontological-concealment-of-failure]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/fidelity-illusion.md|fidelity-illusion]]
- [[entities/surface-completeness-misreading.md|surface-completeness-misreading]]
- [[entities/swe-gate.md|swe-gate]]
- [[entities/legibility-interpretability-gap.md|legibility-interpretability-gap]]

## 📐 개념

- [[concepts/recompilability-preservation-gap.md|recompilability-preservation-gap]]
- [[concepts/fluent-failure-masking.md|fluent-failure-masking]]
- [[concepts/failure-visibility-spectrum.md|failure-visibility-spectrum]]
- [[concepts/meaning-insensitive-metric.md|meaning-insensitive-metric]]
- [[concepts/ontological-concealment-of-failure.md|ontological-concealment-of-failure]]
- [[concepts/execution-verification.md|execution-verification]]
- [[concepts/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/fidelity-illusion.md|fidelity-illusion]]

---
_LLM 분석으로 생성됨_
