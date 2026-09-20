# How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates?

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-21
**링크**: http://arxiv.org/abs/2609.20814v1

## 💡 핵심 인사이트

사전학습 이득은 분포 이동의 성분 분해와 조건 일치 비교를 전제로만 측정 가능하며, 이동 성분별로 사전학습의 데이터 효율 가치가 달라진다.

## 📖 분석

본 논문은 신경 PDE 서러게이트의 사전학습 이득이 분포 이동의 성분별로 조건부임을 실증한다. 한 에어포일 계열의 254,909개 RANS 해로 사전학습한 뒤, 자유류 범위를 일치시킨 두 목표 설정—동일 Spalart-Allmaras(SA) 모델링과 e^N 전이 모델링이 추가된 SA—로 미세조정하여 N=1000 수준에서 사전학습 모델의 신규 CFD 데이터 절감 이득을 확인한다. [[shift-component-decomposition]] 관점에서 기하학적 이동(에어포일 계열 변경)과 물리 모델링 이동(SA→SA+전이)의 효과가 분리 가능함을 보이며, [[distribution-shift]] 논의를 OPTED의 자기유발 이동에 이어 '이동 성분 분해'라는 제3 축으로 확장한다. [[matched-condition-comparison]]은 혼재 변수를 제거하는 쌍별 실험 설계의 PDE 도메인 구현으로 기능하고, [[transfer-learning]]과 [[data-efficiency-gains-from-pretraining]]의 유효 조건을 이동 성분으로 조건화할 것을 요구한다. 이는 사전학습의 가치가 이동 종류와 무관한 보편 속성이 아니라 성분별 재평가 대상임을 시사한다.

## 🔗 관련 논문

- How Does Distribution Shift Shape Pretraining Gains in Neural PDE Surrogates
- OPTED: On-Policy Fine-Tuning for End-to-End Driving using a Render-Fre
- How Does Distribution Shift Shape Pretraining Gains in Neura

## 🏷️ 엔티티

- [[entities/neural-pde-surrogate.md|neural-pde-surrogate]]
- [[entities/shift-component-decomposition.md|shift-component-decomposition]]
- [[entities/matched-condition-comparison.md|matched-condition-comparison]]
- [[entities/distribution-shift.md|distribution-shift]]
- [[entities/transfer-learning.md|transfer-learning]]
- [[entities/data-efficiency-gains-from-pretraining.md|data-efficiency-gains-from-pretraining]]

## 📐 개념

- [[concepts/distribution-shift-component-conditional-pretraini.md|distribution-shift-component-conditional-pretraining-gain]]
- [[concepts/physics-modeling-shift-vs-geometry-shift.md|physics-modeling-shift-vs-geometry-shift]]
- [[concepts/data-efficiency-as-transfer-metric.md|data-efficiency-as-transfer-metric]]
- [[concepts/matched-condition-causal-isolation.md|matched-condition-causal-isolation]]

---
_LLM 분석으로 생성됨_
