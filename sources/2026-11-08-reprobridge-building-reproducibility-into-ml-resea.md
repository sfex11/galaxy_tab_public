# ReproBridge: Building Reproducibility into ML Research Artifacts

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08452v1

## 💡 핵심 인사이트

재현의 성패는 에이전트의 채우기 능력이 아니라 복구된 절차와 결정의 표준화된 보존 여부에 달려 있으며, 복구 노동의 아티팩트 자산화가 재현성을 '일회성 능력'에서 '지속 누적 인프라'로 전환한다.

## 📖 분석

# ReproBridge: Building Reproducibility into ML Research Artifacts

ML 실험 재현은 논문·코드·부속 아티팩트에 흩어진 정보에서 절차를 재구성하는 작업이다. 본 논문은 코딩 에이전트의 재현 성패가 방출 아티팩트 자체보다 누락된 세부를 채우는(fill-in) 능력에 의존한다는 진단에서 출발해, **복구된 절차와 결정을 보존하면 후속 독립 재현이 개선되는가**를 실증한다. 정제된 코드베이스·환경 명세·절차 문서로 구성된 표준화된 아티팩트 설계를 제안하여, 재현 노동의 산물이 일회성 실행 로그가 아닌 축적 가능한 지식 자산이 되도록 한다.

## Wiki 관계

- [[concepts/scientific-finding-reproducibility.md|scientific finding reproducibility]]: 재현성의 질문을 "에이전트가 재현할 수 있는가"에서 "복구 지식이 어떻게 지속 가능한가"로 이동시킨다. 재현 성패가 에이전트 능력이 아니라 복구 산출물의 보존 여부에 조건부임을 확정한다.
- [[concepts/document-centric-research-infrastructure.md|document centric research infrastructure]]: [[entities/intern-atlas.md|intern atlas]]가 방법론 관계 그래프를 제공했다면 본 논문은 아티팩트가 복구된 재현 절차의 운반체로 기능함을 추가하고, 인프라 소비자에 '재현 에이전트'를 명시한다.
- [[concepts/specification-incompleteness-propagation.md|specification incompleteness propagation]]: 불완결 명세가 하류로 전파되는 병리에 복구 결정의 아티팩트 역주입이라는 차단 경로를 제공한다.
- [[entities/ideaambig.md|ideaambig]]: IdeaAMBIG이 아이디어→명세 간극을 측정 진단한다면, 본 논문은 방출 아티팩트→재현 간극을 복구 아티팩트로 메우는 해법 축이다.
- [[entities/rapid.md|rapid]]·[[concepts/reproducible-specification-generation.md|reproducible specification generation]]: 시연→테스트 명세 컴파일(RAPID)과 설계 문서→재생성 원천(Design Docs)과 동형으로, 암묵적 복구 노동을 표준화·재사용 가능한 아티팩트로 컴파일하는 패턴을 재현 도메인에서 확정한다.

## 🔗 관련 논문

- ReproBridge: Building Reproducibility into ML Research Artifacts
- Intern-Atlas: A Methodological Evolution Graph as Research Infrastructure
- IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research Ideas
- RAPID: Robot Agentic Programming from Demonstrations
- Design Docs Are All You Need: An AI-native Machine-Learning Performance
- Scientist World: Grow a Research World for AI-Scientists

## 🏷️ 엔티티

- [[entities/reprobridge.md|reprobridge]]
- [[entities/scientific-finding-reproducibility.md|scientific-finding-reproducibility]]
- [[entities/document-centric-research-infrastructure.md|document-centric-research-infrastructure]]
- [[entities/specification-incompleteness-propagation.md|specification-incompleteness-propagation]]
- [[entities/ideaambig.md|ideaambig]]
- [[entities/intern-atlas.md|intern-atlas]]
- [[entities/rapid.md|rapid]]
- [[entities/reproducible-specification-generation.md|reproducible-specification-generation]]

## 📐 개념

- [[concepts/standardized-artifact-design.md|standardized-artifact-design]]
- [[concepts/recovered-procedure-preservation.md|recovered-procedure-preservation]]
- [[concepts/reproduction-work-compounding.md|reproduction-work-compounding]]
- [[concepts/scientific-finding-reproducibility.md|scientific-finding-reproducibility]]
- [[concepts/document-centric-research-infrastructure.md|document-centric-research-infrastructure]]

---
_LLM 분석으로 생성됨_
