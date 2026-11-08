# Latent Reasoning in Continuous Space for Unified Multimodal Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-11-03
**링크**: http://arxiv.org/abs/2610.42149v1

## 💡 핵심 인사이트

추론(이산 토큰 공간)과 생성(연속 잠재 공간)의 표현 공간 불일치가 UMM의 CoT 활용 실패의 근본 원인이며, 추론을 연속 공간으로 이동시키면 텍스트 번역을 우회하여 LLM의 테스트타임 스케일링과 정밀 제어 가능성이 이미지 생성으로 상속된다.

## 📖 분석

# Latent Reasoning in Continuous Space for Unified Multimodal Models

통합 멀티모달 모델(UMM)이 이미지 생성에서 언어 CoT를 활용하지 못하는 원인을 **모달리티 불일치**로 진단한다 — 추론은 이산 토큰 공간, 생성은 연속 잠재 공간에서 이루어지므로 번역 경계에서 스케일링 이득과 정밀 제어가 소실된다. 해법으로 추론 자체를 연속 공간에서 수행하는 패러다임을 제시한다.

이 진단은 [[concepts/thinking-acting-gap.md|thinking acting gap]]과 동형이다. Continuous Actions from Discrete Minds가 자율주행에서 '이산 토큰 추론 vs 연속 물리 동역학'의 표현 형식 차이를 간극의 근원으로 특정했다면, 본 논문은 이미지 생성에서 동일 구조를 확인해 간극의 도메인 불변성을 강화한다.

[[concepts/latent-visual-reasoning.md|latent visual reasoning]]과 쌍을 이룬다 — VideoLVR이 시각 증거의 잠재 주입으로 '지각→추론' 방향 텍스트 번역 우회를 열었다면, 본 논문은 '추론→생성' 역방향을 열어 우회 원리가 이해 입력과 생성 출력 양단 모두에서 성립함을 완성한다.

[[concepts/cot-as-translated-report.md|cot as translated report]] 관점에서 번역 비용의 조건을 명시한다. 이산 CoT가 텍스트 작업에서 관용적이었다면, 수신자가 연속 공간에서 작동할 때는 번역 자체가 구조적 병목이 된다.

함의: [[concepts/test-time-scaling.md|test time scaling]]이 표현 호환 조건 하에 이미지 생성으로 상속 가능해진다. 동시에 연속 공간 추론의 채택은 [[concepts/unwritten-reasoning-surveillance-exclusion.md|unwritten reasoning surveillance exclusion]]과 [[concepts/credit-decomposition-target-erasure.md|credit decomposition target erasure]]를 생성 도메인으로 확대시킨다.

## 🔗 관련 논문

- VideoLVR: Latent Visual Reasoning over Grounded Video Evidence
- Continuous Actions from Discrete Minds: Latent-Aligned Planning for End-to-End Driving
- Continuous Latent Diffusion Language Model
- Paint-Anything: Unified Any-Color Control for Image Generation and Editing

## 🏷️ 엔티티

- [[entities/unified-multimodal-model.md|unified-multimodal-model]]
- [[entities/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[entities/cot-as-translated-report.md|cot-as-translated-report]]
- [[entities/thinking-acting-gap.md|thinking-acting-gap]]
- [[entities/test-time-scaling.md|test-time-scaling]]
- [[entities/continuous-latent-diffusion.md|continuous-latent-diffusion]]
- [[entities/unified-generation-editing.md|unified-generation-editing]]
- [[entities/multimodal-llm.md|multimodal-llm]]
- [[entities/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]

## 📐 개념

- [[concepts/modality-mismatch-reasoning-generation.md|modality-mismatch-reasoning-generation]]
- [[concepts/continuous-latent-reasoning.md|continuous-latent-reasoning]]
- [[concepts/latent-visual-reasoning.md|latent-visual-reasoning]]
- [[concepts/cot-as-translated-report.md|cot-as-translated-report]]
- [[concepts/thinking-acting-gap.md|thinking-acting-gap]]
- [[concepts/test-time-scaling.md|test-time-scaling]]
- [[concepts/discrete-continuous-adaptation-transition.md|discrete-continuous-adaptation-transition]]
- [[concepts/visual-memory-textual-collapse.md|visual-memory-textual-collapse]]
- [[concepts/irreducible-reconstruction-loss.md|irreducible-reconstruction-loss]]
- [[concepts/unwritten-reasoning-surveillance-exclusion.md|unwritten-reasoning-surveillance-exclusion]]
- [[concepts/credit-decomposition-target-erasure.md|credit-decomposition-target-erasure]]
- [[concepts/observation-point-relocation.md|observation-point-relocation]]

---
_LLM 분석으로 생성됨_
