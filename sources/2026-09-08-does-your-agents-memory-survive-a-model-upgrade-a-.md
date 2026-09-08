# Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study of Memory Portability

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-08
**링크**: http://arxiv.org/abs/2609.05339v1

## 💡 핵심 인사이트

에이전트의 기억은 저장 데이터가 아니라 저장 데이터와 해석 모델 간의 관계이므로, 저장소를 그대로 보존해도 해석기를 교체하면 기억은 소멸한다 — 메모리 이식성은 형식 선택의 문제이며 원본 증거의 보존 정도가 이를 결정한다.

## 📖 분석

모델 업그레이드는 루틴이 되었지만 메모리 이전은 그렇지 않다 — 본 논문은 동일한 메모리 저장소가 모델 교체만으로 '잊어버릴' 수 있음을 통제 실험으로 입증한다. 핵심 진단은 메모리가 저장된 데이터가 아니라 '저장 데이터 × 해석 모델'의 관계라는 점이다: 새 모델은 옛 노트를 다르게 읽고, 임베딩 버전이 혼재하면 검색이 깨지며, 원본 증거 없이는 복구(repair)가 실패한다. 동일한 역사를 4가지 표현으로 보존하는 조건 — LC-RAW(원문 그대로의 장기 컨텍스트), RAG(청킹 검색), NOTES(모델 압축 자연어 노트), 구조화 정규화 — 을 비교하여 충실도·효율성·이식성 사이의 트레이드오프를 최초로 정량화한다. 이 발견은 [[frozen-model-external-memory-contradiction]]가 예견한 모순이 모델 교체 순간에 드러나는 실증 사례이며, [[memory-management]]의 '지식 상태 연속성' 논의를 세션 내 누적에서 모델 버전 간 경계로 확장한다. 또한 [[semantics-aware-checkpoint]]의 '의존 근원 보존' 원리가 메모리 형식 선택에도 성립함을 보여주고, [[adaptive-validity]]의 타당성 조건에 해석기 버전이라는 새 축을 추가한다. 에이전트 인프라 전반에서 '저장과 해석의 분리'가 불완전하다는 통찰의 메모리 도메인 발현이다.

## 🔗 관련 논문

- ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge Work
- Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes
- Rethinking Memory as Continuously Evolving Connectivity
- Novel Memory Forgetting Techniques for Autonomous AI Agents
- Language Models Need Sleep

## 🏷️ 엔티티

- [[entities/memory-management.md|memory-management]]
- [[entities/frozen-model-external-memory-contradiction.md|frozen-model-external-memory-contradiction]]
- [[entities/adaptive-validity.md|adaptive-validity]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/long-context.md|long-context]]
- [[entities/semantics-aware-checkpoint.md|semantics-aware-checkpoint]]
- [[entities/knowledge-loss-translation.md|knowledge-loss-translation]]

## 📐 개념

- [[concepts/memory-portability.md|memory-portability]]
- [[concepts/model-upgrade-forgetting.md|model-upgrade-forgetting]]
- [[concepts/memory-representation-spectrum.md|memory-representation-spectrum]]
- [[concepts/descriptive-decisional-memory-divergence.md|descriptive-decisional-memory-divergence]]

---
_LLM 분석으로 생성됨_
