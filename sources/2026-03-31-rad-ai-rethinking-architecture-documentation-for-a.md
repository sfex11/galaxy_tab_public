# RAD-AI: Rethinking Architecture Documentation for AI-Augmented Ecosystems

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-31  
**링크**: None

## 핵심 요약

**RAD-AI**는 AI 증강 생태계(스마트시티, 자율주행 등)를 위한 아키텍처 문서화 프레임워크이다. 기존 arc42와 C4 모델은 확정적(deterministic) 소프트웨어용으로 설계되어 AI의 확률적 행동, 데이터 의존적 진화, ML/SW 이중 생명주기를 문서화할 수 없다. RAD-AI는 arc42에 8개 AI 전용 섹션, C4에 3개 다이어그램 확장을 추가하여 **EU AI Act Annex IV 준수율을 약 36%에서 93%로 향상**시켰다. Uber Michelangelo, Netflix Metaflow 등 실제 플랫폼 분석을 통해 기존 프레임워크가 놓치는 8가지 AI 고유 관심사를 식별했다.

## 인사이트

1. 기존 아키텍처 문서화 도구(arc42, C4)는 AI 시스템의 확률적 동작과 데이터 의존성을 구조적으로 표현할 수 없어, EU AI Act 같은 규제 준수에 심각한 공백이 존재한다.
2. **연쇄적 드리프트(cascading drift)** 와 **차별화된 규제 의무** 등 생태계 수준의 문제는 기존 표기법으로는 아예 보이지 않는 사각지대에 해당한다.
3. RAD-AI는 기존 프레임워크와 **하위 호환성**을 유지하면서 확장하는 방식이므로, 실무 도입 장벽을 크게 낮출 수 있다.

## 응용 가능성

1. **고위험 AI 시스템 규제 대응**: 2026년 8월 EU AI Act 시행을 앞두고, RAD-AI를 활용하면 Annex IV 기술 문서화 요건을 체계적으로 충족할 수 있다.
2. **대규모 AI 플랫폼 거버넌스**: 복수의 ML 모델이 상호작용하는 생태계(자율주행, 스마트시티 등)에서 모델 간 의존성·드리프트·생명주기를 통합 관리하는 문서화 표준으로 활용할 수 있다.

## 추출된 엔티티

_없음_

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-31-RAD-AIRethinkingArchitectureDo.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-01-rad-ai-rethinking-architecture-documentation-for-a.md]]
