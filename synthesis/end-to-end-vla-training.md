# End To End Vla Training: 합성 분석

**생성일**: 2026-09-07  
**관련 논문**: 3편  
**최종 업데이트**: 2026-09-07

# End To End Vla Training: 합성 분석

> **수집 범위**: 2026-09-06 ~ 09-07, 3편 (LaPla 2편은 동일 논문 arXiv:2609.04070의 중복 수집으로, 실질 2편)

## 📌 핵심 발견

이번 수집은 end-to-end VLA 훈련이 [[entities/vla-foundry.md|vla-foundry]]가 정의한 로봇 조작에서 **자율주행이라는 연속적·물리제약 도메인으로 확장**되는 전환점을 포착한다. 두 논문은 각각 알고리즘 계층과 실험 인프라 계층을 담당한다.

**1. 표현 형식이 간극을 결정한다 (LaPla)**
LaPla는 VLM의 이산 추론과 차량 연속 동역학 사이 간극을 능력 문제가 아닌 **표현 형식의 비동형성** 문제로 재정의한다. 잔차 [[concepts/vector-quantization.md|vector-quantization]] 기반 액션 토크나이저가 차량 kinematics를 이산 토큰으로 인코딩하되 연속성 정밀도를 보존하고, latent-aligned planning이 의미 공간과 실행 공간을 잠재 차원에서 정렬한다. [[concepts/tokenization.md|tokenization]]은 압축 기법에서 '물리 제약의 이산 인코딩'이라는 표현 계약으로 격상되며, [[concepts/semantic-id-tokenization.md|semantic-id-tokenization]]과 함께 '비텍스트 대상의 이산 토큰화'라는 공통 패턴을 형성한다.

**2. 병목은 알고리즘이 아니라 인프라다 (미니어처 플랫폼)**
저비용 Ackermann 차량과 Webos 디지털 트윈의 쌍 구성([[concepts/physical-digital-twin-pairing.md|physical-digital-twin-pairing]])은 [[concepts/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]를 개인 연구자 수준으로 민주화한다. 연속 제약 도메인으로 확장된 VLA 훈련에 시뮬레이션 사전 검증-실차 실행의 이중 루프라는 실증 무대를 제공한다.

## 🔗 논문 간 관계

- **모순**: 없음. 두 논문은 상호 배타적 계층을 다룬다.
- **보완**: LaPla가 '표현 계층'(행동을 어떻게 토큰화할 것인가)을, 플랫폼이 '검증 계층'(어디서 닫힌 루프로 평가할 것인가)을 담당한다. 플랫폼의 [[concepts/command-conditioned-behavior-cloning.md|command-conditioned-behavior-cloning]] 기준선 위에 잠재 정렬 정책을 탑재하는 것이 자연스러운 후속 실험이다.
- **공통 전제**: [[entities/thinking-acting-gap.md|thinking-acting-gap]]과 [[entities/representation-action-gap.md|representation-action-gap]]이 도구 호출을 넘어 물리 도메인에서도 유효하다는 진단. [[entities/closed-loop-evaluation.md|closed-loop-evaluation]]을 모두 암묵적 목표로 한다.

## 📈 트렌드와 미래 방향

1. **도메인 불변성 검증**: VLA 패러다임이 조작→주행으로 확장되며, 항공·수중 등 추가 도메인 확장이 예상된다.
2. **토큰화의 보편 인터페이스화**: 콘텐츠(semantic ID)와 행동(action token)을 아우르는 이산 인터페이스로 수렴.
3. **연구 민주화**: [[concepts/miniaturization-accessibility.md|miniaturization-accessibility]]와 [[concepts/open-experimental-platform.md|open-experimental-platform]]이 진입 장벽을 하향 평준화.
4. **후속 과제**: 미니어처 플랫폼에서의 잠재 정렬 실증, 잠재 인터페이스의 물리적 안전성 검증, sim-to-real 간극의 정량적 측정.

> **종합**: VLA 훈련의 성숙은 '표현 형식의 질'(소프트웨어)과 '검증 인프라의 접근성'(하드웨어)의 동시 진보로 규정된다.