# Measurement-Driven Sub-Network Selection for On-Premise Retrieval-Augmented Factory Agents

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-04
**링크**: http://arxiv.org/abs/2609.02760v1

## 💡 핵심 인사이트

압축과 검색 그라운딩 적응을 거친 후에는 모델 크기가 태스크 품질을 예측하지 못하므로, 배포는 크기 기반 사전 추론이 아닌 적응 후 측정 기반 선택 문제가 된다.

## 📖 분석

# Measurement-Driven Sub-Network Selection for On-Premise Retrieval-Augmented Factory Agents (2026-09-04)

## 핵심 발견: 크기의 예측력 붕괴

온프레미스 공장 에이전트 배포 연구로, 유능한 모델이 현장 하드웨어에 맞지 않는 문제를 다룬다. 핵심 실증: 구조적 압축([[model-compression]]) 후 검색 그라운딩 적응([[retrieval-augmented-generation]])을 거치면 **모델 크기가 적응 후 응답 품질을 예측하지 못한다**. 일반 능력은 파라미터 수에 거의 선형으로 감소하지만, 판정 기반 RAG 응답 품질은 그렇지 않다. 이는 [[accuracy-safety-scaling-divergence]]의 정확도-안전성 발산과 동형인 '일반 능력-태스크 품질' 스케일링 발산 사례로, [[scaling-laws]]의 '크기→능력' 단조성 전제가 적응 후 태스크 품질에서는 성립하지 않음을 보여준다.

## 배포의 재정의: 적응 후 선택

방법론적 기여는 배포를 "적응 전 크기 기반 추론"이 아닌 "적응 후 측정 기반 서브네트워크 선택"으로 재정의한 것이다. [[measurement-architecture-misattribution]]이 지적한 '점수=본질 능력' 오류의 역방향 적용으로, 크기 프록시 대신 실측 품질로 후보를 선별해야 한다.

## Wiki 연결

- [[marginal-distribution-ceiling]]: 검색 그라운딩이 조건부 최적화를 통해 소형 모델의 태스크 도달 범위를 대형 모델 수준으로 재배치할 수 있음을 시사
- [[on-device-inference]]: 상점 바닥 하드웨어 제약이 연구 동기
- [[cost-aware-agent-evaluation]]: '비용 예산 내 안전'과 동형인 '하드웨어 예산 내 품질' 평가 축
- "When Does Bigger Help"(2026-09-02)와 대화 형성: 크기 확장의 이득 조건을 태스크·적응 조건부로 세분화

## 🔗 관련 논문

- When Does Bigger Help: A Controlled Study of LLM Scaling
- Carbon-Taxed Transformers: A Green Compression Pipeline
- Select to Think: Unlocking SLM Potential with Local Sufficiency

## 🏷️ 엔티티

- [[entities/model-compression.md|model-compression]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/retrieval-augmented-generation.md|retrieval-augmented-generation]]
- [[entities/post-adaptation-selection.md|post-adaptation-selection]]

## 📐 개념

- [[concepts/capability-task-quality-decoupling.md|capability-task-quality-decoupling]]
- [[concepts/marginal-distribution-ceiling.md|marginal-distribution-ceiling]]
- [[concepts/measurement-architecture-misattribution.md|measurement-architecture-misattribution]]
- [[concepts/accuracy-safety-scaling-divergence.md|accuracy-safety-scaling-divergence]]
- [[concepts/cost-aware-agent-evaluation.md|cost-aware-agent-evaluation]]

---
_LLM 분석으로 생성됨_
