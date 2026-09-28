# Compact Documentation for Coding Agents: A Benchmark, an Optimizer, and Why It Does Not Transfer

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31587v1

## 💡 핵심 인사이트

코드 설명의 충실도는 길이가 아닌 완전성이 결정하며, 테스트 기반 라운드트립으로 완전 충실도에 도달한 문서조차 에이전트의 실제 이슈 해결 성능으로 전이되지 않는다 — 재생성 가능성과 수행 지원성은 분리된 속성이다.

## 📖 분석

**Compact Documentation for Coding Agents (2026-09-29)**

자연어 문서화가 코딩 에이전트의 소프트웨어 이슈 해결에 실제로 도움이 되는지 검증하는 연구. 핵심 도구는 **라운드트립 벤치마크**다 — 코드 설명으로부터 코드를 재생성하고, 재생성 코드가 원본 테스트를 통과하는지로 설명의 충실도를 채점한다. 실행 기반 검증이 문서라는 텍스트 산출물의 품질 측정에도 적용됨을 보여준다([[executable-benchmark]], [[verification-as-system-external-relation]]).

두 가지 발견:
1. **완전성 > 길이**: 설명 충실도를 결정하는 것은 길이가 아니라 완전성이다. '압축 문서화' 전제(짧을수록 충분하다)가 기각되며, 토큰 절감과 정보 충실도가 직교함을 시사한다([[token-efficiency]], [[compression-forgetting-isomorphism]]).
2. **전이 실패**: 벤치마크를 최적화 신호로 삼아 설명 작성 프롬프트를 자동 발견하면 완전 충실도에 도달하고 미개지 파일로 일반화되지만, 그 이득은 실제 에이전트의 이슈 해결 성능으로 전이되지 않는다.

2번이 핵심이다. 재생성 충실도(프록시)와 에이전트 수행 지원(실제 목표)의 단절은 [[evaluation-target-substitution]]·[[one-shot-gain-fallacy]]의 문서화 도메인 발현이며, [[swe-gate]]의 '테스트 통과 ≠ 수용 가능' 진단과 동형이다. Design Docs 계열의 전제 — 문서가 재생성의 단일 진실원이라는([[design-doc-primacy]]) — 명제를 [[ideaambig]]·[[reproducible-specification-generation]]의 축에서 정량 검증한다: 명세는 재생성 가능해질 수 있으나, 에이전트 하네스([[interpretive-harness]])로 기능하는 것은 별개의 속성이다.

## 🔗 관련 논문

- Design Docs Are All You Need: An AI-native Machine-Learning Performance Auditor
- IdeaAMBIG: Benchmarking Implementation-Critical Gaps in Research-Idea Specs
- SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineer Agents
- ExecCritic: Learn to Test, Test to Improve for Coding Agents

## 🏷️ 엔티티

- [[entities/compact-documentation-coding-agents.md|compact-documentation-coding-agents]]
- [[entities/executable-benchmark.md|executable-benchmark]]
- [[entities/evaluation-target-substitution.md|evaluation-target-substitution]]
- [[entities/one-shot-gain-fallacy.md|one-shot-gain-fallacy]]
- [[entities/token-efficiency.md|token-efficiency]]
- [[entities/prompt-engineering.md|prompt-engineering]]
- [[entities/reproducible-specification-generation.md|reproducible-specification-generation]]
- [[entities/interpretive-harness.md|interpretive-harness]]
- [[entities/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[entities/single-surface-signal-insufficiency.md|single-surface-signal-insufficiency]]

## 📐 개념

- [[concepts/roundtrip-benchmark.md|roundtrip-benchmark]]
- [[concepts/documentation-completeness-over-length.md|documentation-completeness-over-length]]
- [[concepts/proxy-transfer-failure.md|proxy-transfer-failure]]

---
_LLM 분석으로 생성됨_
