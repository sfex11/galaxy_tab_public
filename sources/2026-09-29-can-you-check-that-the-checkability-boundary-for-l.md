# Can You Check That? The Checkability Boundary for Local LLM Network Automation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-29
**링크**: http://arxiv.org/abs/2609.31540v1

## 💡 핵심 인사이트

과제가 저비용 결정론적 검사를 노출하는 순간 프라이버시(데이터 국소성)와 신뢰성(품질 게이트)은 트레이드오프가 아닌 동시 달성 가능한 속성이 되며, 검증 불가능성만이 민감 데이터의 프론티어 위임을 정당화하는 유일한 근거로 남는다.

## 📖 분석

네트워크 자동화 입력(운영 설정·토폴로지·로그)을 제3자 프론티어 LLM에 보내면 민감 아티팩트가 유출되고, 로컬 SLM은 오류가 잦다는 딜레마에서 출발해 **검증 가능성(checkability)**을 로컬 추론 적용 가능 과제를 결정하는 기준으로 제시한다. 과제가 위반 출력을 기각하는 저비용·결정론적 내재적 검사를 노출하면, SLM 출력을 검사로 게이팅하여 프라이버시와 품질을 동시에 담보할 수 있다.

기존 Wiki와의 관계: [[rlvr]]이 검증 가능성을 훈련 보상 신호로 사용했다면 본 논문은 같은 속성을 배포 시점 추론 라우팅 판단 기준으로 전용하며, 검증 가능성이 모델 출력과 독립적인 시스템-외부 관계라는 [[verification-as-system-external-relation]] 명제를 네트워크 도메인에서 재확인한다. [[computation-unit-meta-selection]]의 SLM vs LLM 선택에 '검증 가능성 × 데이터 민감도'라는 원리적 판정 기준을 부여하고, [[non-cognitive-oracle]]의 환경 인과 사실 기반 검증과 동형을 이룬다. [[slm-reasoning-gap]]에는 능력 향상이나 추론 제거가 아닌 '격차가 품질을 훼손하지 않는 과제의 선별'이라는 제3 경로([[local-sufficiency]] 계열)를 제공하며, [[on-device-inference]]의 적용 범위를 '검증 가능한 과제에서 품질 손실 없는 대안'으로 재정의한다. 프라이버시 접근으로서는 통계적 난독화([[differential-privacy]])가 아닌 데이터 신뢰 경계 내 유지라는 구조적 격리 계열에 속한다.

## 🔗 관련 논문

- SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the S
- Large Language Models (LLMs) for Telecom Root Cause Analysis (RCA): A
- Select to Think: Unlocking SLM Potential with Local Sufficie
- Verifier-Backed Hard Problem Generation for Mathematical Rea
- Verifiable by Construction: Claim-Level Evaluation of Verbatim Citatio

## 🏷️ 엔티티

- [[entities/checkability-boundary.md|checkability-boundary]]
- [[entities/rlvr.md|rlvr]]
- [[entities/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[entities/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[entities/slm-reasoning-gap.md|slm-reasoning-gap]]
- [[entities/on-device-inference.md|on-device-inference]]
- [[entities/inference-privacy.md|inference-privacy]]
- [[entities/data-exfiltration-prevention.md|data-exfiltration-prevention]]
- [[entities/non-cognitive-oracle.md|non-cognitive-oracle]]
- [[entities/local-sufficiency.md|local-sufficiency]]
- [[entities/capability-safety-inseparability.md|capability-safety-inseparability]]
- [[entities/statistical-certification.md|statistical-certification]]

## 📐 개념

- [[concepts/intrinsic-check.md|intrinsic-check]]
- [[concepts/deployment-time-verifiability.md|deployment-time-verifiability]]
- [[concepts/privacy-driven-inference-partitioning.md|privacy-driven-inference-partitioning]]
- [[concepts/verification-as-system-external-relation.md|verification-as-system-external-relation]]
- [[concepts/computation-unit-meta-selection.md|computation-unit-meta-selection]]
- [[concepts/non-cognitive-oracle.md|non-cognitive-oracle]]

---
_LLM 분석으로 생성됨_
