# MedGraph: Maintaining Patient State with Graph Memory for Long-Term Medical Dialogue

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-08
**링크**: http://arxiv.org/abs/2611.08433v1

## 💡 핵심 인사이트

장기 의료 대화에서 메모리 실패는 낡은 상태(staleness)·타인 사실 혼입(contamination)·안전 사실 결여(omission)의 3원으로 귀결되며, 날짜가 붙은 사실의 그래프화가 이 세 축을 동시에 관리하는 최소 구조다.

## 📖 분석

MedGraph는 환자를 방문마다 따라가는 의료 어시스턴트를 위해, 임상 상태 변화에도 정확성을 유지하는 그래프 메모리를 제시한다. 5개 메모리 시스템의 longitudinal 오류 분석에서 세 가지 반복 원인 — 검색 증거가 낡은 상태를 주는 staleness, 타인의 건강 사실 혼입인 cross-person contamination, 답변이 의존하는 안전 사실의 결여인 safety omission — 를 규명하고, 세션별 날짜가 붙은 사실 추출로 그래프를 구축해 세 실패 모드에 동시 대응한다.

이 3원 분류는 [[adaptive-validity]]의 임상 실증이다: 모델 업그레이드와 환경 변화에 이어 '환자 상태 변화'라는 제3의 메모리 무효화 원천을 추가하며, staleness는 [[revisit-time-validity-observation]]의 재방문 시점 타당성 문제를 정량화한 구현이다. 날짜 속성의 일급 부여는 [[epistemic-bookkeeping]]의 시간축을 도메인에서 실현한다.

[[clinical-graph-learning]]이 EEG 신호 그래프의 위상 정제를 다뤘다면, 본 논문은 대화 사실에서 환자 상태 그래프를 구축하는 쌍대 축을 제공해 임상 그래프의 원료가 신호에서 대화로 확장됨을 보여준다. [[knowledge-state-orchestration]]의 지식 상태 장부가 ADEMA에서 추상적이었다면, 환자 상태라는 도메인 인스턴스로 구체화된다. [[speaker-attributed-memory]]가 '누가 말했는가'를 추적했다면, MedGraph는 '누구에 관한 사실인가'의 오귀속이 의료 도메인의 치명적 실패 모드임을 보여준다.

## 🔗 관련 논문

- A Living Benchmark for Information Retrieval from Electronic Health Records
- HealthNLP_Retrievers at ArchEHR-QA 2026: Cascaded LLM Pipeline
- SpeakerMem-R1: Speaker-Centered Dual-Track Memory for Multi-Party Dialogue
- ADEMA: A Knowledge-State Orchestration Architecture for Long-Horizon Knowledge
- LLM as Clinical Graph Structure Refiner: Enhancing Representation Learning
- Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study

## 🏷️ 엔티티

- [[entities/medgraph.md|medgraph]]
- [[entities/clinical-graph-learning.md|clinical-graph-learning]]
- [[entities/ehr-question-answering.md|ehr-question-answering]]
- [[entities/medical-ai.md|medical-ai]]

## 📐 개념

- [[concepts/patient-state-memory.md|patient-state-memory]]
- [[concepts/adaptive-validity.md|adaptive-validity]]
- [[concepts/cross-person-fact-contamination.md|cross-person-fact-contamination]]
- [[concepts/safety-fact-omission.md|safety-fact-omission]]
- [[concepts/knowledge-state-orchestration.md|knowledge-state-orchestration]]
- [[concepts/speaker-attributed-memory.md|speaker-attributed-memory]]
- [[concepts/epistemic-bookkeeping.md|epistemic-bookkeeping]]
- [[concepts/ehr-question-answering.md|ehr-question-answering]]

---
_LLM 분석으로 생성됨_
