# A Low-Cost, Open Platform for End-to-End Autonomous Driving on a Miniature Ackermann Vehicle

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-06
**링크**: http://arxiv.org/abs/2609.04147v1

## 💡 핵심 인사이트

미니어처 규모의 개방형 물리 플랫폼은 시뮬레이션-실세계 간극을 고비용 장벽 없이 검증 가능한 연구 인프라로 전환하여, 체화 자율주행 연구의 민주화와 sim-to-real 검증 경로를 동시에 실현한다.

## 📖 분석

본 논문은 Webots 디지털 트윈과 소형 Ackermann 차량을 결합한 저비용 개방형 자율주행 실험 플랫폼을 제시한다. 인쇄된 도시 트랙, 데이터 수집·궤적 등록 도구를 포함하여 시뮬레이션 기반 방법론과 실세계 실행을 연결하는 통제 실험을 가능하게 한다. 기존 Wiki의 [[sandbox-liveworld-gap]]이 통제 환경 평가와 실세계 배포의 단절을 진단했다면, 본 플랫폼은 미니어처 규모에서 이 간극을 명시적으로 가교하는 인프라적 해법이다. command-conditioned behavior cloning 베이스라인이 시뮬레이션 학습 정책의 실차 검증 경로를 실증하며, [[closed-loop-evaluation]] 논의의 물리적 실현 사례가 된다. LiDAR 인지 중심의 기존 [[autonomous-driving]] 논의(Toward Robust LiDAR Semantic Segmentation)를 end-to-end 정책 연구 인프라로 확장하고, [[agent-environment-generation]]이 소프트웨어 환경 생성에 집중한 것과 대비되는 체화적([[embodied-ai]]) 환경 구축 경로를 보여준다. 저비용 개방성은 자율주행 연구의 진입 장벽이 고비용 실차 실험이라는 암묵적 전제를 해체하며, SafetyALFRED가 지적한 disembodied 평가 한계를 실물 환경 실험으로 보완할 기반을 제공한다.

## 🔗 관련 논문

- Toward Robust LiDAR Semantic Segmentation for Real-World Dep
- SafetyALFRED: Evaluating Safety-Conscious Planning of Multimodal Large
- Three-Step Nav: A Hierarchical Global-Local Planner for Zero

## 🏷️ 엔티티

- [[entities/autonomous-driving.md|autonomous-driving]]
- [[entities/embodied-ai.md|embodied-ai]]
- [[entities/sandbox-liveworld-gap.md|sandbox-liveworld-gap]]
- [[entities/agent-environment-generation.md|agent-environment-generation]]
- [[entities/closed-loop-evaluation.md|closed-loop-evaluation]]
- [[entities/miniature-vehicle-research-platform.md|miniature-vehicle-research-platform]]

## 📐 개념

- [[concepts/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]
- [[concepts/miniaturization-accessibility.md|miniaturization-accessibility]]
- [[concepts/physical-digital-twin-pairing.md|physical-digital-twin-pairing]]

---
_LLM 분석으로 생성됨_
