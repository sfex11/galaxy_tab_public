# Seeing Before Synthesizing: VLM-Guided Transition Event Discovery for Weakly-Supervised Dense Video Captioning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-07
**링크**: http://arxiv.org/abs/2609.04183v1

## 💡 핵심 인사이트

훈련 감독 신호의 품질은 합성 모델의 언어 능력이 아니라, 합성에 앞서 무엇을 얼마나 정확히 관찰했는가에 의해 결정된다.

## 📖 분석

## Seeing Before Synthesizing (SBS)

Weakly-Supervised Dense Video Captioning에서 최근 LLM 합성 transition 캡션이 시각적 근거 없이 모든 사건 간 갭에 고정 위치·길이로 부여되는 관행을 진단하고, VLM 기반 관찰을 선행시켜 transition 이벤트를 적응적으로 발견·제공하는 프레임워크를 제안한다.

### 기존 Wiki 개념과의 관계
- [[blind-tool-invocation]]: 시각 검증 없이 합성 캡션을 훈련에 투입하는 것은 blind invocation의 파이프라인 버전으로, '사용 전 검증' 원칙이 도구 호출을 넘어 훈련 데이터 생성으로 확장된다.
- [[circular-validity-problem]]: 합성 데이터가 감독 신호가 되면 타당성이 생성 가설에만 의존하는 순환 구조가 생기며, SBS는 VLM 관찰이라는 외부 근거 주입으로 이 루프를 절단한다.
- [[fixed-assignment-fragility]]: 고정 갭 할당의 구조적 취약성을 명시하고 그 대안 설계의 동기를 제공한다.

### 새 축
- [[adaptive-transition-discovery]], [[vision-grounded-synthesis]], [[synthetic-grounding-gap]]

### 연결점
ShallowStream의 지연 실행(얕은 인덱스→깊은 응답), Validation-Driven LLM Workflows의 검증 기반 정제와 함께, 비디오 이해와 생성 워크플로우 연구가 '언제 무엇을 볼 것인가'의 문제로 수렴함을 시사한다.

## 🔗 관련 논문

- ShallowStream: Index Shallow then Answer Deep for Streaming Video Understanding
- Generating Statistical Charts with Validation-Driven LLM Workflows

## 🏷️ 엔티티

- [[entities/adaptive-transition-discovery.md|adaptive-transition-discovery]]
- [[entities/vision-grounded-synthesis.md|vision-grounded-synthesis]]
- [[entities/synthetic-grounding-gap.md|synthetic-grounding-gap]]
- [[entities/fixed-assignment-fragility.md|fixed-assignment-fragility]]
- [[entities/blind-tool-invocation.md|blind-tool-invocation]]
- [[entities/circular-validity-problem.md|circular-validity-problem]]
- [[entities/video-understanding.md|video-understanding]]

## 📐 개념

- [[concepts/seeing-before-synthesizing.md|seeing-before-synthesizing]]
- [[concepts/weakly-supervised-dense-video-captioning.md|weakly-supervised-dense-video-captioning]]
- [[concepts/visual-grounding.md|visual-grounding]]
- [[concepts/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[concepts/transition-event-discovery.md|transition-event-discovery]]

---
_LLM 분석으로 생성됨_
