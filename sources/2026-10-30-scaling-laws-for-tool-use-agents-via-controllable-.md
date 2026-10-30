# Scaling Laws for Tool-Use Agents via Controllable Environment Synthesis

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-30
**링크**: http://arxiv.org/abs/2610.37648v1

## 💡 핵심 인사이트

합성 환경의 다양성을 도구·태스크·데이터베이스라는 조작 가능한 3축으로 분해하면, 에이전트 훈련의 스케일링 법칙을 환경 구성 수준에서 측정하고 최적화할 수 있다.

## 📖 분석

본 논문은 도구 사용 에이전트 훈련에서 합성 환경의 데이터 구성이 성능에 미치는 영향을 스케일링 법칙 수준에서 규명한다. SynthAPI 파이프라인은 환경 다양성을 도구·태스크·데이터베이스라는 3축으로 명시적 제어 가능하게 만들고, 458개 환경 변이 실험을 통해 환경 구성이 훈련 효과를 인과적으로 결정함을 실증한다.

Wiki 지형에서 본 논문의 위치는 세 간선으로 요약된다. 첫째, [[agent-environment-generation]] 계보(Gym-Anything의 범용 변환 → [[terminal-universe]]의 궤적 재활용 → CodeMidas의 코드 유래 환경)에 '구성의 체계적 제어' 단계를 추가한다 — 환경을 만드는 것을 넘어 무엇을 어떤 비율로 만들지가 조작 변수가 된다. 둘째, [[implicit-curriculum]]의 데이터 수준 논의를 환경 수준으로 확장하여, 합성 환경의 구성 비율이 에이전트 훈련의 커리큘럼으로 기능함을 보인다. 셋째, [[environment-diversity-layered-guarantee]]가 제기한 '무엇이 다양해야 하는가'의 질문에 3축 분해로 답하여 다양성 설계를 추상적 원칙에서 파라미터 공간으로 전환한다.

[[scaling-laws]] 관점에서 스케일링의 축이 모델 크기·데이터 양에서 환경 구성으로 확장됨을 시사한다. [[envsched]]가 환경의 실행·검증 비용을 다룬다면 본 논문은 그 이전 단계인 공급 구성 설계를 담당하여 환경 인프라 연구의 상류를 채운다. [[verifiable-training-data-synthesis]]와 결합하면, 도구가 데이터베이스 위에서 작동하는 구조 덕에 합성 환경이 검증 가능한 태스크·검증자 쌍을 제공함을 보여준다.

## 🔗 관련 논문

- envsched-environment-aware-scheduling-for-rollout-
- terminal-universe-turning-agent-trajectories-into-
- codemidas-scaling-agentic-coding-rl-environments-f
- environment-evolution-for-terminal-agents

## 🏷️ 엔티티

- [[entities/environment-composition-control.md|environment-composition-control]]
- [[entities/environment-scaling-law.md|environment-scaling-law]]
- [[entities/tool-use-agent-training-data.md|tool-use-agent-training-data]]
- [[entities/scaling-laws.md|scaling-laws]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/environment-diversity-layered-guarantee.md|environment-diversity-layered-guarantee]]
- [[entities/verifiable-training-data-synthesis.md|verifiable-training-data-synthesis]]
- [[entities/environment-supply-scaling.md|environment-supply-scaling]]

## 📐 개념

- [[concepts/synthesis-diversity-axes.md|synthesis-diversity-axes]]
- [[concepts/implicit-curriculum.md|implicit-curriculum]]
- [[concepts/environment-composition-control.md|environment-composition-control]]

---
_LLM 분석으로 생성됨_
