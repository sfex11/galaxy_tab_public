# Design Docs Are All You Need: An AI-native Machine-Learning Performance Tool

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05364v1

## 💡 핵심 인사이트

AI 코드 생성 비용의 붕괴는 소프트웨어 유지보수의 경제학을 역전시켜, 지속 자산의 지위를 코드에서 설계 문서로 이전시킨다 — 코드는 폐기·재생성 가능한 컴파일 산출물이 된다.

## 📖 분석

# Design Docs Are All You Need (SMART, 2026-09-08)

ML 성능 모델링은 장수 소프트웨어에 가장 적대적인 영역이다 — 오늘의 추상화에 구워진 가정이 내일의 모델·시스템에 의해 무효화되어 끝없는 리팩토링을 강요한다. 본 논문은 여기서 경제적 역전을 선언한다: AI 코딩 에이전트가 충분히 빨라져, 점진적 패치의 기술 부채 상환보다 라이브러리 전체를 재생성하는 편이 저렴해졌다. 이에 따라 SMART는 엄밀한 기호적(symbolic) 성능 모델링 라이브러리를 설계 문서로부터 재생성하는 방식으로 구축한다.

## Wiki 맥락

1. **코드의 위상 전환**: [[code-as-agent-harness]]가 하네스를 LLM 생성 코드의 동적 번역 계층으로 재정의했다면, SMART는 그 단위를 전체 라이브러리로 확장해 코드를 설계 문서에서 컴파일되는 일회성 산출물로 격하한다. [[source-level-self-rewriting]](MOSS)의 '소스 수정'과 대비되는 '폐기·재생성' 극점이다.

2. **간극의 재발성**: [[algorithm-system-translation-gap]]과 [[abstraction-layer-mismatch]]의 부정합이 모델·시스템 진화에 의해 구조적으로 재발한다는 전제는, 해법이 추상화 정교화가 아니라 재번역 비용을 상쇄하는 재생성 인프라임을 시사한다.

3. **명세의 일차성**: [[reproducible-specification-generation]]에 '명세→코드베이스 전체 재생성' 소비 측을 추가하고, [[ai-architecture-documentation]]에 문서가 코드보다 오래 사는 종단 사례를 제공한다.

4. **부채의 재평가**: [[regression-tax]]의 소프트웨어 버전 — 기술 부채 상환 비용 — 을 재생성 비용과의 명시적 트레이드오프로 격상시킨다. 에이전트 주도 인프라 구축의 선행 사례 [[design-conductor]]에 '순환적 재구축' 차원을 더한다.

## 신규 개념 제안

- **design-doc-primacy**: 설계 문서가 코드 대신 유일한 진실 원천이 되는 위상 역전
- **regeneration-over-maintenance**: AI 생성 비용 하락으로 '재생성 < 유지보수'가 되는 경제 임계점
- **ai-native-software-lifecycle**: 코드를 일회성 컴파일 산출물로 보는 수명주기 패러다임

## 🔗 관련 논문

- MOSS: Self-Evolution through Source-Level Rewriting in Auton
- From Research Question to Scientific Workflow: Leveraging Agentic AI f
- RAD-AI: Rethinking Architecture Documentation for AI-Augment
- Design Conductor 2.0: An agent builds a TurboQuant inference
- Agentic Harness Engineering: Observability-Driven Automatic

## 🏷️ 엔티티

- [[entities/smart-performance-library.md|smart-performance-library]]
- [[entities/code-as-agent-harness.md|code-as-agent-harness]]
- [[entities/harness-mutability.md|harness-mutability]]
- [[entities/ai-architecture-documentation.md|ai-architecture-documentation]]
- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/abstraction-layer-mismatch.md|abstraction-layer-mismatch]]
- [[entities/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[entities/source-level-self-rewriting.md|source-level-self-rewriting]]
- [[entities/regression-tax.md|regression-tax]]
- [[entities/symbolic-computation.md|symbolic-computation]]
- [[entities/design-conductor.md|design-conductor]]

## 📐 개념

- [[concepts/design-doc-primacy.md|design-doc-primacy]]
- [[concepts/regeneration-over-maintenance.md|regeneration-over-maintenance]]
- [[concepts/ai-native-software-lifecycle.md|ai-native-software-lifecycle]]

---
_LLM 분석으로 생성됨_
