# IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research-Idea Specifications

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-11
**링크**: http://arxiv.org/abs/2609.10539v1

## 💡 핵심 인사이트

연구 아이디어의 신규성과 과학적 타당성은 구현 가능성을 담보하지 않는다 — 명세화 준비도(codification readiness)라는 독립 품질 축을 정량화함으로써, 자율 연구와 코딩 에이전트의 병목이 아이디어 발견에서 명세의 충분성으로 이동함을 규명한다.

## 📖 분석

# IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research-Idea Specifications

## 정의

연구 아이디어가 신규성·일관성·과학적 타당성을 갖추어도 제안된 방법이 충실히 구현될 만큼 명세되지 않을 수 있음을 정량화하는 벤치마크. **명세화 준비도(codification readiness)** — 유능한 구현자 또는 코딩 에이전트가 근거 없는 가정 없이 의도된 방법을 구축하기에 충분한 방법론 정보를 명세가 제공하는가 — 를 평가 대상으로 삼는다. 근거 기반 명세와 그 지원 재구성을 대비 구축해 아이디어-구현 간극을 측정한다.

## 기존 Wiki와의 관계

- [[reproducible-specification-generation]]: Design Docs가 설계 문서를 코드 재생성의 단일 진실원으로 삼았다면, 본 논문은 그 명세가 재생성에 실제로 충분한지 감사하는 품질 축을 제공한다. 명세 중심 패러다임의 필수 보완이다.
- [[scientific-workflow-agent]]: 연구 질문→구조화된 의도→재현 가능한 명세→실행의 3층 아키텍처에서 중간 '명세' 계층의 품질을 독립적으로 측정하는 평가 인프라다.
- [[autoresearch]]: 아이디어 생성과 충실한 구현이 구조적으로 분리된 능력임을 시사하며, artifact-bound-optimization의 대상을 논문 산출물에서 구현 명세로 확장할 축을 연다.
- [[benchmark-specification-gap]]: 벤치마크 명세의 불완전성이 측정 대상을 왜곡하듯 구현 명세의 불완전성이 구현 대상을 왜곡함을 보여 동형 구조를 확장한다.

## 핵심 인사이트

아이디어의 가치와 명세의 완전성은 독립 속성이며, 자율 연구와 코딩 에이전트의 실제 병목은 아이디어 발견이 아닌 명세화에 있다.

## 🔗 관련 논문

- Design Docs Are All You Need: An AI-native Machine-Learning 
- From Research Question to Scientific Workflow: Leveraging Agentic AI f 
- SAEScientist-Bench: Can AI Agents Conduct Autonomous SAE Int
- SWE-Gate: Passing Functional Tests Is Not Enough for Softwar

## 🏷️ 엔티티

- [[entities/ideaambig.md|ideaambig]]
- [[entities/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[entities/scientific-workflow-agent.md|scientific-workflow-agent]]
- [[entities/autoresearch.md|autoresearch]]
- [[entities/benchmark-specification-gap.md|benchmark-specification-gap]]
- [[entities/research-capability-benchmark.md|research-capability-benchmark]]

## 📐 개념

- [[concepts/codification-readiness.md|codification-readiness]]
- [[concepts/implementation-faithfulness.md|implementation-faithfulness]]
- [[concepts/unsupported-assumption.md|unsupported-assumption]]
- [[concepts/idea-implementation-gap.md|idea-implementation-gap]]

---
_LLM 분석으로 생성됨_
