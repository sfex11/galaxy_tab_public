# KV-streams for Efficient Compaction in Agentic Reinforcement Learning

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35750v1

## 💡 핵심 인사이트

압축의 병목은 추론에서는 레이턴시, 훈련에서는 반복 프리필에 의한 처리량으로 이질적으로 발생하므로, 학습 가능한 압축 정책의 성립 조건은 정책 품질이 아니라 정책 훈련의 계산 가능성이며 이는 인프라 층의 문제다.

## 📖 분석

## KV-streams: 애그네틱 RL 훈련을 위한 효율적 컨텍스트 압축

애그네틱 LLM의 장기 지평 확장이 GPU 메모리에 담아야 할 컨텍스트 트레이스 길이에 병목됨을 진단한다. 컨텍스트 압축(compaction)이 메모리를 일정하게 유지하는 표준 해법이지만, 대부분의 압축 전략이 LLM 컨텍스트를 수차례 반복 프리필해야 하여 훈련 처리량을 저해한다는 병인을 제시한다. KV-streams는 반복 프리필을 제거하는 플러그앤플레이 스트리밍 KV 계산 전략으로, 학습 가능한(trainable) 압축을 효율적으로 가능하게 한다.

### 기존 Wiki 논의와의 관계

- [[compactionrl]]: CliffCompaction 계열이 과제 완료 보상으로 압축 정책을 RL 최적화하는 접근을 제시했다면, 본 논문은 그 정책 훈련을 막던 프리필 반복 병목을 제거하는 전제조건을 공급한다. 압축 정책 학습이 이론적 제안에서 실용 경로로 전환되는 계기다.
- CliffCompaction·[[cross-session-compaction]]: 추론 시점 압축이 교차 에피소드 지식 재사용을 담당했다면, 본 논문은 훈련 시점 압축이라는 대응 축을 연다. 압축이 평가·배포(추론)와 롤아웃(훈련) 양축의 공통 인프라가 됨을 보여준다.
- [[kv-cache-optimization]]: KV 캐시 최적화의 범위를 서빙·추론 계층에서 RL 훈련 계층으로 확장하며, 캐시 관리가 학습 처리량의 구성요소임을 규정한다.

### 새 인사이트

압축의 비용 구조는 추론과 훈련에서 다르다 — 추론에서는 레이턴시가, 훈련에서는 프리필 반복에 의한 처리량이 지배적이다. 이 구분 없이는 '효율적 압축'의 설계 목표가 잘못 규정된다. 학습 가능한 압축 정책의 성립 조건은 정책 품질이 아니라 정책 훈련의 계산 가능성이며, 이것이 인프라 층의 문제임을 확정한다.

## 🔗 관련 논문

- CliffCompaction: Cost-Efficient Compaction for Long-Horizon 
- Flash-dLLM: IO-Aware KV Caching and Parallel Decoding for Fa

## 🏷️ 엔티티

- [[entities/compactionrl.md|compactionrl]]
- [[entities/kv-cache-optimization.md|kv-cache-optimization]]
- [[entities/cross-session-compaction.md|cross-session-compaction]]
- [[entities/kv-streams.md|kv-streams]]

## 📐 개념

- [[concepts/trainable-compaction.md|trainable-compaction]]
- [[concepts/prefill-bottleneck.md|prefill-bottleneck]]

---
_LLM 분석으로 생성됨_
