# Autonomous Driving: 합성 분석

**생성일**: 2026-09-07  
**관련 논문**: 4편  
**최종 업데이트**: 2026-09-07

# Autonomous Driving: 합성 분석

> **분석 대상**: 4편 (2026-09-04 ~ 2026-09-07) · LiDAR 강인성 평가, 미니어처 오픈 플랫폼, 헤드랜드 커버리지 계획, LaPla 잠재 정렬 계획

## 공통 주제: 네 층위의 갭

4편의 논문은 자율주행 파이프라인의 서로 다른 층위에서 **성능 자체가 아니라 갭이 병목**이라는 동일한 진단을 내린다.

- **평가-배포 갭**: LiDAR 세그멘테이션 논문은 벤치마크 mIoU가 거친 라벨·악천후·도메인 시프트 앞에서 유지되지 않음을 3축 스트레스 평가로 분해한다. 안전 중요 클래스(보행자·차량) 위상 보존을 별도 축으로 삼아 [[concepts/evaluation-deployment-unit-mismatch.md|evaluation-deployment-unit-mismatch]]의 지각 버전을 확정한다.
- **시뮬-실차 갭**: 미니어처 Ackermann 플랫폼은 병목이 알고리즘이 아닌 실험 인프라 비용임을 진단하고, 물리 차량+Webos 디지털 트윈 쌍으로 [[concepts/sim-to-real-validation-infrastructure.md|sim-to-real-validation-infrastructure]]를 개인 연구자 수준까지 민주화한다([[concepts/miniaturization-accessibility.md|miniaturization-accessibility]]).
- **기동 어휘 갭**: 헤드랜드 커버리지 논문은 코너 미커버의 원인이 파라미터 튜닝 불충분이 아니라 부드러운 회전 클래스 자체의 한계임을 보이고, 후진 기동이라는 행동 공간 확장으로 해소한다.
- **표현 형식 갭**: LaPla는 VLM의 이산 추론과 차량의 연속 운동학 사이 [[concepts/thinking-acting-gap.md|thinking-acting-gap]]을 능력 문제가 아닌 표현 비동형성으로 진단하고, VQ-VAE 액션 토크나이저라는 잠재 공유 인터페이스로 봉합한다.

## 논문 간 관계

**일치**: 네 논문 모두 컴포넌트 내 최적화가 아닌 구조적 개입(평가 프로토콜 재설계, 행동 어휘 확장, 표현 계약 재정의, 인프라 재구축)을 해법으로 삼는다. [[concepts/paradigm-level-adaptive-routing.md|paradigm-level-adaptive-routing]]의 '패러다임 내 최적화 vs 전환' 구분이 자율주행 전 영역에서 유효함을 보여준다.

**보완**: (1) LiDAR 논문(갭 진단)과 미니어처 플랫폼(통제된 실차 재현 인프라)은 스트레스 평가→물리 검증의 파이프라인을 구성한다. (2) Corner Cases(계획층 어휘 확장)와 LaPla(표현층 인터페이스 구축)는 각기 다른 층에서 "행동 가능성 확장"이라는 동일 방향을 취한다.

**긴장(해소 가능)**: LiDAR 논문의 벤치마크 불신과 미니어처 플랫폼의 시뮬 사전검증 신뢰는 표면적 모순이다. 그러나 전자는 절대 성능 주장을, 후자는 통제 조건에서의 상대 비교를 다루며, 시뮬레이션의 역할이 "성능 예측"에서 "구조적 실패의 조기 발견"으로 재정의되면 양립한다.

## 트렌드와 미래 방향

1. **SOTA 추격 → 갭 과학**: 정확도 경쟁에서 실패 조건의 분해·정량화로 연구 중심이 이동 중.
2. **인프라 민주화**: 저비용 오픈 플랫폼이 갭 진단을 소규모 연구자에게 개방한다.
3. **도로 밖 확장**: 농경지 사례는 자율주행이 field robotics로 확장되며 기동 어휘 요구가 도메인마다 다름을 시사한다.
4. **VLA 수렴**: LaPla와 미니어처 플랫폼의 결합은 [[entities/end-to-end-vla-training.md|end-to-end-vla-training]]에 통제된 실증 무대를 제공한다.

**차세대 과제**: 스트레스 평가 프로토콜 + 디지털 트윈 검증 + 확장 행동 어휘 + 잠재 정렬 인터페이스를 통합한 **풀스택 배포 준비성 검증**. 특히 [[concepts/safety-critical-control.md|safety-critical-control]] 관점에서 지각층 위상 보존(LiDAR)이 계획층 행동 확장(Corner Cases)과 상호작용하는 경로를 추적하는 종단 간 실험이 요구된다.