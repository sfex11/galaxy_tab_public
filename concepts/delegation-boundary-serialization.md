# Delegation Boundary Serialization

**생성일**: 2026-05-02

## 정의

의미론적 의존 그래프의 엣지에 소유권(ownership)과 위임 경계(delegation boundary)를 메타 속성으로 부착하여, 체크포인트 시 위임 상태 자체가 직렬화 대상이 되고 복원 시 위임 일관성이 검증되어야 한다는 설계 원칙. 단일 에이전트에서는 모든 상태 노드가 암묵적으로 하나의 주체에 귀속되므로 불필요했던 속성.

## 관련 논문

- agent-sandbox-state-management
- agora-opt

---
_자동 Wiki Query에서 추출됨_

### Crab: A Semantics-Aware Checkpoint/Restore Runtime for Agent Sandboxes (2026-05-03)
