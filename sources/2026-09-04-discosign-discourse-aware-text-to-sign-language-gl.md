# DiscoSign: Discourse-Aware Text to Sign Language Gloss Translation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02796v1

## 💡 핵심 인사이트

문장 수준 처리 단위는 담화 수준의 언어 구조와 구조적으로 부정합하며, 공간 앵커링 같은 담화 상태의 일관성을 명시적 모듈로 다루는 것이 도메인 충실한 번역의 전제다.

## 📖 분석

DiscoSign은 수어 글로스 번역에서 문장 수준 처리의 한계를 넘어 담화(discourse) 현상을 일급 처리 대상으로 삼는다. 모듈형 LLM 파이프라인 안에서 공간 지시 해소(spatial coreference resolution) 등 세 가지 담화 현상을 명시적으로 다루며, 설계는 언어학 연구에 기반한다.

Wiki 관점에서 이 논문의 기여는 두 층위다. 첫째, 처리 단위의 구조적 부정합([[abstraction-layer-mismatch]])을 번역 도메인에서 실증한다: 문장 단위 운영은 담화 수준 구조를 필연적으로 파괴하며, 이는 [[token-step-pipeline-hierarchy]]가 문서화한 입도 부정합 패턴의 언어학적 변형이다. 둘째, 공간 지시 해소는 개체의 공간 위치라는 상태가 담화 전체에서 일관되게 유지되어야 하는 지식 상태 관리 문제로, 첫 언급에서 설정된 공간 앵커가 이후 모든 참조의 의존 기반이 되는 [[semantic-dependency-graph]]를 형성한다. 이는 ADEMA 계열의 [[knowledge-state-orchestration]]과 동형 구조를 언어 처리 도메인에서 보여준다. 주목할 점은 긴 컨텍스트 주입이 아닌 명시적 구조 모듈로 교차 문장 의존성을 처리한다는 점이다.

나아가 도메인 지식(언어학)이 시스템 설계 구조를 결정하는 [[natural-language-to-formal-language]] 방향의 성공 사례이며, 형식 문법 기반 번역 평가 연구(Evaluating In-Context Translation)와 담화 수준에서 접점을 가진다.

## 🔗 관련 논문

- LLM as Clinical Graph Structure Refiner: Enhancing Representation Lear

## 🏷️ 엔티티

- [[entities/discourse-aware-translation.md|discourse-aware-translation]]
- [[entities/spatial-coreference-resolution.md|spatial-coreference-resolution]]
- [[entities/sign-language-gloss-translation.md|sign-language-gloss-translation]]
- [[entities/llm.md|llm]]

## 📐 개념

- [[concepts/discourse-state-consistency.md|discourse-state-consistency]]
- [[concepts/sentence-discourse-granularity-gap.md|sentence-discourse-granularity-gap]]

---
_LLM 분석으로 생성됨_
