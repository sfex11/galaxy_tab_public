# Breaking the Uniformity Trap: Scaling Video Diffusion Model via SplitMoE

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-01
**링크**: http://arxiv.org/abs/2609.38140v1

## 💡 핵심 인사이트

전문가 사용의 균등성 정규화는 준균질 토큰 분포를 가진 LLM에 맞춘 설계 유산이며, 시공간적으로 중복되고 의미적으로 롱테일인 비디오 데이터에서는 라우팅의 의미 조직화를 훼손하는 균등성 트랩으로 작동한다.

## 📖 분석

## SplitMoE: 균등성 트랩을 깨는 비디오 확산 MoE 스케일링

MoE 스케일링 패러다임을 비디오 확산 모델로 확장하면서, 기존 시각 MoE가 **균등성 트랩(uniformity trap)**에 빠져 있음을 진단한다. 토큰별 독립 라우팅과 균등 전문가 사용 정규화는 [[mixture-of-experts]]의 LLM 유산인데, 시공간적으로 중복되고 의미적으로 롱테일 분포를 따르는 비디오 데이터에서는 오히려 의미적으로 조직화되지 않은 라우팅을 강화한다. SplitMoE는 전문가 분할을 통해 라우팅을 데이터의 의미 구조에 정렬시켜 이를 회피한다.

**기존 Wiki와의 관계**: [[mixture-of-experts]] 엔티티는 지금까지 LLM 맥락에서 축적되었다 — EMO의 사전학습 창발적 모듈성, Nemotron 계열의 경쟁 프로그래밍 실증. 본 논문은 그 스펙트럼을 시각 생성으로 확장하되 중요한 반전을 추가한다. [[pretraining-induced-expert-specialization]]이 전문가 특화의 창발을 긍정했다면, 본 논문은 균등성 정규화가 그 창발을 구조적으로 억제할 수 있음을 보여 특화의 성립 조건을 명시한다.

**연결점**: [[video-inference-efficiency]]가 추론 효율 메커니즘 지형을 정리한 것과 상보적으로, 본 논문은 스케일링(훈련 측) 축에서 데이터 분포와 아키텍처 정규화의 정렬을 다룬다. TIDE([[expert-placement-as-compression]])가 MoE 확산 LLM 추론의 배치 문제였다면, 본 논문은 비디오 확산의 전문가 조직 문제로 도메인과 축을 모두 확장한다.

## 🔗 관련 논문

- EMO: Pretraining Mixture of Experts for Emergent Modularity
- TIDE: Efficient and Lossless MoE Diffusion LLM Inference with Expert Offloading
- Why Is Video Still So Expensive? A Survey of Inference-Efficiency Mechanisms

## 🏷️ 엔티티

- [[entities/mixture-of-experts.md|mixture-of-experts]]
- [[entities/video-diffusion.md|video-diffusion]]
- [[entities/splitmoe.md|splitmoe]]

## 📐 개념

- [[concepts/uniformity-trap.md|uniformity-trap]]
- [[concepts/semantic-expert-organization.md|semantic-expert-organization]]
- [[concepts/load-balancing-regularization.md|load-balancing-regularization]]
- [[concepts/pretraining-induced-expert-specialization.md|pretraining-induced-expert-specialization]]

---
_LLM 분석으로 생성됨_
