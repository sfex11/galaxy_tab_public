# Cross-Agent Checkpoint Consistency

**생성일**: 2026-05-02

## 정의

다중 에이전트가 독립적으로 체크포인트를 생성할 때 발생하는 인과적 비일관성 문제. 에이전트 A가 t=10에, 에이전트 B가 t=12에 체크포인트를 찍고, t=8에 메시지 교환이 있었다면 CP_A는 이를 포함하지만 CP_B는 포함하지 않아 동시 복원 시 인과성이 위배된다. 단일 에이전트 Crab이 보장하는 '의미론적 의존 그래프의 동일 재구성'이 부분 순서(partial order) 문제로 변형되는 지점.

## 관련 논문

- algorithm-system-translation-gap
- agent-sandbox-state-management
- checkpoint-restore-efficiency-spectrum

---
_자동 Wiki Query에서 추출됨_
