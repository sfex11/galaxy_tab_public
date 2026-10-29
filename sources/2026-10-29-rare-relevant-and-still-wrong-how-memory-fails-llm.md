# Rare, Relevant, and Still Wrong: How Memory Fails LLM Group Decisions

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37624v1

## 💡 핵심 인사이트

그룹 논의를 위한 기억 압축에서 희귀성·관련성 휴리스틱 모두 실패하는 근본 원인은 정보의 보유 빈도가 결정 가치와 자연스럽게 혼재되어 있기 때문이며, 소유권을 분리한 진단 벤치마크만이 이 혼재를 측정 가능하게 만든다.

## 📖 분석

### Rare, Relevant, and Still Wrong: How Memory Fails LLM Group Decisions (2026-10-29)

LLM 그룹의 논의를 최종 의사결정자에게 전달할 짧은 기억으로 압축할 때 무엇을 남길 것인가라는 질문에 답한다. '가장 희귀한 주장 보존'과 '결정 기준 관련성 보존'이라는 두 자연스러운 휴리스틱이 히든 프로파일 과제에서 모두 실패함을 보인다 — 정보의 보유 빈도(얼마나 널리 알려져 있는가)와 결정 가치(도움이 되는가)가 자연 데이터에서 혼재(confounded)되어 있기 때문이다. 희귀한 미끼(decoy)는 희귀성 휴리스틱을 속이고, 널리 보유된 지지 증거의 가치는 관련성 필터에 의해 가려진다.

이는 retention-proxy-mismatch의 그룹 의사결정 실증이다. CliffCompaction·kv-streams 계열이 압축 정책을 과제 보상으로 학습했다면, 본 논문은 그 이전 질문 — 희귀성·관련성 같은 표면 프록시가 왜 실패하는가 — 을 진단하며 descriptive-decisional-memory-divergence을 정량적으로 확정한다. 기억의 결정 가치는 보유 빈도나 명시 기준 일치가 아니라 decision-critical-evidence 소유 구조에 있다.

CrossProfile은 60개 템플릿에 자동 검증 정답 키를 갖춘 진단 벤치마크로, 지지·미끼·무관 정보의 소유권을 분리한다. 이는 matched-condition-comparison 원리를 기억 선택 평가에 이식한 설계이며, 자동 검증 키는 verifiable-training-data-synthesis 원리의 평가 응용이다. belief-aggregation 연구가 최빈값 수렴을 보였다면, 본 논문은 집계 이전의 압축 계층이 어떤 그룹 신념이 생존할지 결정하는 상류 병목임을 밝혀, 집합 의사결정 연구의 초점을 '어떻게 합칠까'에서 '무엇이 합쳐지기 전에 사라지는가'로 이동시킨다.

## 🔗 관련 논문

- Multi-agent Scaling Across Disjunctive and Compensatory Tasks
- CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents
- KV-streams for Efficient Compaction in Agentic Reinforcement Learning

## 🏷️ 엔티티

- [[entities/crossprofile-benchmark.md|crossprofile-benchmark]]
- [[entities/retention-proxy-mismatch.md|retention-proxy-mismatch]]
- [[entities/descriptive-decisional-memory-divergence.md|descriptive-decisional-memory-divergence]]
- [[entities/decision-critical-evidence.md|decision-critical-evidence]]
- [[entities/matched-condition-comparison.md|matched-condition-comparison]]
- [[entities/belief-aggregation.md|belief-aggregation]]
- [[entities/non-selective-context-accumulation.md|non-selective-context-accumulation]]
- [[entities/future-query-agnostic-compression.md|future-query-agnostic-compression]]
- [[entities/information-preservation-boundary.md|information-preservation-boundary]]
- [[entities/aggregate-vs-emergent-collaboration-gap.md|aggregate-vs-emergent-collaboration-gap]]

## 📐 개념

- [[concepts/rarity-relevance-confound.md|rarity-relevance-confound]]
- [[concepts/hidden-profile-memory-failure.md|hidden-profile-memory-failure]]
- [[concepts/decision-oriented-memory-selection.md|decision-oriented-memory-selection]]

---
_LLM 분석으로 생성됨_
