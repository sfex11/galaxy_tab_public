# Epistemic Infrastructure (인식론적 인프라)

**분야**: AI Knowledge Management
**생성일**: 2026-04-14

## 정의

기업 AI 지식 시스템이 단순 검색(retrieval)을 넘어, 지식의 **확정 상태/신뢰 등급/쟁점 여부**를 추적하고 관리하는 구조. "Retrieval Is Not Enough" 논문이 제안한 개념으로, Wiki 97편 종합 결과 4개 계층으로 구성됨.

## Wiki에서 도출된 4개 계층

### 1. 거버넌스 계층
- [[entities/llm-agent|Governed Memory]]: 지식 생성·수정·폐기 규칙 통일
- 메모리 사일로, 거버넌스 파편화, 품질 저하 문제 식별

### 2. 동기화 계층
- PSI: 공유 상태 버스로 모듈 간 추론과 동기화
- Triadic Cognitive Architecture: **인식론적 마찰(epistemic friction)** — LLM의 '인지적 무중력'을 아키텍처 수준에서 제어

### 3. 신뢰 추적 계층
- Dynamic Belief Graphs: 믿음을 시간에 따라 진화하는 그래프로 모델링
- VL-Calibration: 지각 실패와 추론 오류를 분리하여 신뢰도 보정
- MemBoost: 불확실성 기반 에스컬레이션 (확신 낮으면 상위 모델로 위임)

### 4. 감사 계층
- SCRAT: 검증 가능하고 감사 가능한 궤적 (verifiable/auditable trajectories)
- DAO Belief Aggregation: 집단적 지식 결정의 신뢰 등급 부여

→ [[queries/query-2.md|상세 분석]]

## 관련 논문
- 
- 
- 
- 

---
_Wiki Query 결과에서 새로운 개념으로 추출됨 (2026-04-14)_
