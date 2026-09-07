# Reinforcement Learning: 합성 분석

**생성일**: 2026-09-07  
**관련 논문**: 8편  
**최종 업데이트**: 2026-09-07

# Reinforcement Learning: 합성 분석

**생성일**: 2026-07-27
**관련 논문**: 8편 등록 (고유 4편 — 중복 4편 정리)
**최종 업데이트**: 2026-12-01
**변경 사항**: 신규 논문 없음. 중복 등록 정리, 수명 주기 관점 심화, 절단되었던 개념 섹션 복원

## 공통 주제: 배포 가능한 RL의 세 가지 근원적 난제

고유 4편은 "벤치마크 점수를 넘어선 신뢰성"이라는 메타 주제로 수렴한다.

**비정상성.** 드리프트·마모로 동역학이 진화하는 환경을 다루는 GP 기반 Continual MBRL과, sim-to-real 간극을 다루는 진화적 RL은 정상성(stationarity) 가정의 붕괴라는 동일 근원을 공유하며, 모두 이를 분포 이동의 변주로 규정한다.

**검증의 부재.** 심볼릭 속성 분석은 점 속성(point properties) 검증으로는 전체 상태 공간에서의 DRL 행동을 보장할 수 없다는 진단에서 출발한다. 적응형 비디오 스트리밍·혼잡 제어 등 임계 인프라 적용이 이 병목의 실무적 무게를 보여준다.

**훈련 비효율.** Android Coach는 SSSA(단일 상태-단일 행동) 패러다임과 에뮬레이터 지연이 겹친 구조적 샘플 낭비를 스냅샷 복원 기반 SSMA 분기 탐색으로 해소한다.

## 논문 간 관계: 긴장, 통합, 상충

**MB vs. MF 로버스트니스 긴장.** GP-MBRL은 동역학의 명시적 모델링으로 적응하고, CEM-DDPG/TD3는 집단 탐색으로 암묵적 강건성을 확보한다. 같은 문제에 정반대 경로를 택하며, 명시적 모델의 추정 오류 vs. 암묵적 탐색의 샘플 비용이라는 트레이드오프가 미해결이다.

**탐색의 3차원 통합 가능성.** CEM(정책 파라미터 공간), SSMA(상태-행동 공간 분기), GP 불확실성(동역학 공간)이 서로 다른 차원에서 탐색을 공격한다. 불확실성이 높은 상태에서 SSMA 분기 샘플을 CEM 집단 적합도 평가에 주입하는 통합 아키텍처가 단일 차원 탐색의 한계를 넘을 후보다.

**세팅 상충과 수명 주기.** SSMA의 스냅샷 분기는 환경 가역성을 전제로 하므로, 가역성 없는 물리 환경의 MBRL·ERL과 직접 결합되지 않는다. 그럼에도 효율적 훈련(Android Coach) → 전역 검증(심볼릭 분석) → 운영 중 적응(GP-MBRL) → 재강건화(진화적 RL)로 이어지는 수명 주기 파이프라인 관점이 성립한다.

## 연구 트렌드와 미해결 과제

**시스템 중심 RL로의 이동.** 에뮬레이터 지연·스냅샷, 네트워크 인프라, 비정상 동역학 등 도메인 제약이 RL 파이프라인에 역주입되며, 범용 알고리즘에서 파라다임 특화로 이동한다. Android 에이전트 연구는 RL과 [[concepts/computer-use-agent.md|computer-use agent]] 연구의 접점을 제공하며, 관련 LLM 가드레일 연구(TraceSafe)와의 수렴도 주목된다.

**미해결 과제.** ① MB+진화적 RL 하이브리드 아키텍처의 부재, ② 고차원 상태 공간에서 심볼릭 검증의 계산 확장성, ③ 비가역 환경에서의 SSMA 대체 기법, ④ 세 차원 탐색을 아우르는 통합 이론.

## 📐 관련 개념

- [[concepts/reinforcement-learning.md|reinforcement-learning]]
- [[concepts/distribution-shift.md|distribution-shift]]
- [[concepts/model-based-rl.md|model-based-rl]]
- [[concepts/world-model.md|world-model]]
- [[concepts/meta-learning.md|meta-learning]]
- [[concepts/model-predictive-control.md|model-predictive-control]]
- [[concepts/formal-verification.md|formal-verification]]
- [[concepts/ai-safety.md|ai-safety]]
- [[concepts/agent-reliability-auditing.md|agent-reliability-auditing]]
- [[concepts/token-efficiency.md|token-efficiency]]
- [[concepts/computer-use-agent.md|computer-use-agent]]
- [[concepts/embodied-ai.md|embodied-ai]]
- [[concepts/metaheuristic-optimization.md|metaheuristic-optimization]]

---
_LLM 분석으로 재생성됨_