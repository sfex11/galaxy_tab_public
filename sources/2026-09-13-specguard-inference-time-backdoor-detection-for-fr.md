# SpecGuard: Inference-Time Backdoor Detection For Free

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-13
**링크**: http://arxiv.org/abs/2609.11799v1

## 💡 핵심 인사이트

추측 디코딩의 수락/거부 신호를 재용도하여 백도어 탐지를 서빙 비용과 분리함으로써, 지연 민감 배포 환경에서도 비용 0의 지속 런타임 감시가 성립함을 입증한다.

## 📖 분석

SpecGuard는 LLM 서빙 인프라의 기존 신호를 재용도하여 추가 추론 비용 없이('For Free') 배포 모델의 백도어를 런타임에 탐지한다. 백도어는 정상 입력에서 은닉되어 있다가 비밀 트리거 출현 시에만 공격자 제어 행동으로 전환되므로 사전 감사만으로는 잦은 업데이트 모델을 보호할 수 없으나, 기존 추론 시점 탐지기는 트리거 구조 가정이나 지연 민감 서빙과 충돌하는 추가 계산을 요구했다.

본 논문은 [[free-security-observability]]의 대표적 실현이다. 감시를 서빙 최적화의 부산물로 전환하여 보안-효율 트레이드오프([[zero-sum-optimization-trap]])를 구조적으로 해소하고, [[infrastructure-sensor-duality]]의 '운영 텔레메트리 이중 기능'을 백도어 도메인에서 확정한다. [[speculative-decoding]] 계열([[speckv]])이 개척한 내부 상태 관측과 동일 접점에 놓이며, [[certification-monitoring-discontinuity]]의 단절을 비용 0의 지속 감시로 메운다. [[serving-safety-coupling]]의 긍정적 극 — 서빙 아키텍처가 안전의 병목이 아니라 감지 기반으로 기능함 — 을 입증한다.

다만 [[sensor-as-attack-surface]]의 역설이 적용된다: 수락/거부 신호가 백도어 센서로 공개되면, 적대자는 해당 신호를 정상 범위로 유지하도록 다음 세대 백도어를 설계할 것이다. 무료 관측 가능성이 곧 적대적 최적화 표면이 되는 구조적 긴장을 내포하며, [[threat-defense-surface-identity]]의 또 다른 발현이다.

## 🔗 관련 논문

- SpecKV: Adaptive Speculative Decoding with Compression-Aware Gamma Sel
- FL-PBM: Pre-Training Backdoor Mitigation for Federated Learn

## 🏷️ 엔티티

- [[entities/backdoor-attack.md|backdoor-attack]]
- [[entities/speculative-decoding.md|speculative-decoding]]
- [[entities/speckv.md|speckv]]
- [[entities/free-security-observability.md|free-security-observability]]
- [[entities/runtime-verification-layer.md|runtime-verification-layer]]
- [[entities/serving-safety-coupling.md|serving-safety-coupling]]
- [[entities/infrastructure-sensor-duality.md|infrastructure-sensor-duality]]
- [[entities/certification-monitoring-discontinuity.md|certification-monitoring-discontinuity]]
- [[entities/zero-sum-optimization-trap.md|zero-sum-optimization-trap]]
- [[entities/threat-defense-surface-identity.md|threat-defense-surface-identity]]
- [[entities/sensor-as-attack-surface.md|sensor-as-attack-surface]]

## 📐 개념

- [[concepts/serving-safety-coupling.md|serving-safety-coupling]]
- [[concepts/infrastructure-sensor-duality.md|infrastructure-sensor-duality]]
- [[concepts/certification-monitoring-discontinuity.md|certification-monitoring-discontinuity]]
- [[concepts/zero-sum-optimization-trap.md|zero-sum-optimization-trap]]
- [[concepts/threat-defense-surface-identity.md|threat-defense-surface-identity]]
- [[concepts/sensor-as-attack-surface.md|sensor-as-attack-surface]]
- [[concepts/free-security-observability.md|free-security-observability]]

---
_LLM 분석으로 생성됨_
