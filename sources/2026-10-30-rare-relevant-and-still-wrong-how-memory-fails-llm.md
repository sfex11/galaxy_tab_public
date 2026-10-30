# Rare, Relevant, and Still Wrong: How Memory Fails LLM Group Decisions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37624v1

## 💡 핵심 인사이트

메모리 압축에서 희귀성과 관련성이라는 직관적 보존 휴리스틱은 사실의 소유 분포와 결정 가치가 혼동되는 숨은 프로필 조건에서 결정적으로 중요한 지지 증거를 체계적으로 놓치며, 이 실패는 소유 구조를 분리하는 검증 가능한 벤치마크로만 진단 가능하다.

## 📖 분석

본 논문은 LLM 그룹 논의를 최종 결정자용 단기 메모리로 압축할 때 '무엇을 보존할 것인가'의 문제를 진단한다. 희귀한 주장을 보존하거나 결정 기준과 관련된 주장을 보존하는 두 직관적 휴리스틱은 숨은 프로필(hidden-profile) 태스크에서 모두 실패한다 — 사실이 얼마나 널리 보유되는가와 그것이 결정에 도움이 되는가가 혼동되기 때문이다. 저자는 자동 검증된 정답 키를 갖춘 60개 템플릿의 [[crossprofile-benchmark]]를 도입하여 지지·미끼·무관 정보를 소유 구조로 분리하고, 두 휴리스틱 모두 결정적으로 중요한 지지 증거를 놓침을 실증한다.

Wiki 관점에서 이 논문은 [[descriptive-decisional-memory-divergence]]의 경험적 구현체다 — 묘사적 보존 지표(희귀성·관련성)가 결정적 가치를 담보하지 못함을 검증 가능한 형태로 정량화한다([[retention-proxy-mismatch]], [[rarity-relevance-confound]]). 또한 [[decision-critical-evidence]]의 존재론을 확장한다: 최종 결정자가 유지해야 할 증거의 범위는 논의 참여자들의 보유 분포와 구조적으로 다르며, 이 간극이 압축 계층의 명시적 관리 대상이 된다([[information-preservation-boundary]]). 압축 시점에 최종 결정을 알 수 없는 조건은 [[future-query-agnostic-compression]]의 그룹 의사결정 버전이며, CliffCompaction 계열이 단일 에이전트 컨텍스트 압축을 다뤘다면 본 논문은 다중 참여자→단일 결정자 구조의 압축 실패로 [[aggregate-vs-emergent-collaboration-gap]]에 측정 계층을 제공한다. [[hidden-profile-memory-failure]] 관점에서 '희귀 사실 우대'라는 직관이 오히려 미끼 선택을 강화하는 역설이 핵심 발견이다.

## 🔗 관련 논문

- CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents
- Towards Communication-Efficient Social Intelligence in Language Agents
- Scaling Long-Form Story Generation via Narrative State Tracking

## 🏷️ 엔티티

- [[entities/crossprofile-benchmark.md|crossprofile-benchmark]]
- [[entities/retention-proxy-mismatch.md|retention-proxy-mismatch]]
- [[entities/rarity-relevance-confound.md|rarity-relevance-confound]]
- [[entities/decision-critical-evidence.md|decision-critical-evidence]]
- [[entities/future-query-agnostic-compression.md|future-query-agnostic-compression]]
- [[entities/aggregate-vs-emergent-collaboration-gap.md|aggregate-vs-emergent-collaboration-gap]]
- [[entities/hidden-profile-memory-failure.md|hidden-profile-memory-failure]]
- [[entities/descriptive-decisional-memory-divergence.md|descriptive-decisional-memory-divergence]]

## 📐 개념

- [[concepts/information-preservation-boundary.md|information-preservation-boundary]]
- [[concepts/decision-oriented-memory-selection.md|decision-oriented-memory-selection]]

---
_LLM 분석으로 생성됨_
