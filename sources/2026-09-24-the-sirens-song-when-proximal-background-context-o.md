# The Sirens' Song: When Proximal Background Context Overshadows Distant Evidence

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-24
**링크**: http://arxiv.org/abs/2609.26718v1

## 💡 핵심 인사이트

장기 컨텍스트에서 원거리 증거 회수 실패의 진짜 원인은 거리가 아니라 과업 무관 근접 배경의 누적 경쟁이며, 해법은 위치 기반이 아닌 꼬리 무거운 내용 기반 정렬(LYRA)에 있다.

## 📖 분석

본 논문은 장기 컨텍스트 LLM의 원거리 증거 회수 실패에 대한 진단을 재작성한다. 거리 자체가 원인이라는 기존 설명을 기각하고, 과업 무관 근접 배경(요약문·반복 패턴 등 풍부한 근접 텍스트)이 원거리 증거와 누적적으로 경쟁하여 주의를 익사시키는 'Proximity Trap'을 제시하며, t-분포 기반 방향성 매칭(LYRA)으로 소수의 진짜 관련 증거가 억압되지 않도록 관련성 점수의 꼬리를 무겁게 정렬한다.

Wiki와의 핵심 연결은 세 가지다. 첫째, [[attention-self-concentration]]·[[attention-sink]]와의 구조적 평행 — 'It's Not RoPE'가 어텐션 싱크의 위치 인코딩 설명을 기각하고 자기 집중으로 재귀인했다면, 본 논문은 원거리 실패의 거리(위치) 설명을 기각하고 내용 기반 경쟁으로 재귀인하여, 어텐션 병리 진단에서 위치 귀인 배제라는 방법론적 흐름을 확정한다. 둘째, [[bottleneck-misattribution]]의 어텐션 내부 사례 — '거리가 병목'이라는 표면 진단 대신 근접 무관 배경 경쟁이 실제 병목임을 실증한다. 셋째, [[long-context]] 진화 선상에서 LongSeeker·ShallowStream류 지연 실행·얕은 인덱스 전략이 유효한 병인을 규정한다 — 길이 자체가 아니라 근접 노이즈의 익사 효과 때문이다. [[confident-failure-predictability]]에는 근접 배경 밀도라는 실행 전 관측 가능한 실패 예측 변수를 추가한다.

## 🔗 관련 논문

- It's Not RoPE that Creates Sinks: The Role of Self-Concentration and Value Non-Mixing
- Predictable Failure in Multi-Hop Retrieval: Score-Distribution
- LongSeeker: Elastic Context Orchestration for Long-Horizon Search Agents
- On-Demand Attention: Language Models Know When to Recall

## 🏷️ 엔티티

- [[entities/proximity-trap.md|proximity-trap]]
- [[entities/lyra.md|lyra]]
- [[entities/long-context.md|long-context]]
- [[entities/attention-self-concentration.md|attention-self-concentration]]
- [[entities/attention-sink.md|attention-sink]]
- [[entities/bottleneck-misattribution.md|bottleneck-misattribution]]
- [[entities/confident-failure-predictability.md|confident-failure-predictability]]
- [[entities/on-demand-attention.md|on-demand-attention]]

## 📐 개념

- [[concepts/proximity-trap.md|proximity-trap]]
- [[concepts/proximal-background-competition.md|proximal-background-competition]]
- [[concepts/heavy-tailed-relevance-matching.md|heavy-tailed-relevance-matching]]
- [[concepts/positional-attribution-rejection.md|positional-attribution-rejection]]

---
_LLM 분석으로 생성됨_
