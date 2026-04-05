# UI-Voyager: A Self-Evolving GUI Agent Learning via Failed Experience

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-03-27  
**링크**: None

## 핵심 요약

UI-Voyager는 모바일 GUI 자동화를 위한 **2단계 자기진화 에이전트**다. 1단계에서는 **Rejection Fine-Tuning(RFT)**을 통해 외부 개입 없이 학습 데이터와 모델이 자율적으로 공진화하는 루프를 구축한다. 2단계에서는 **Group Relative Self-Distillation(GRSD)**을 도입하여, 그룹 롤아웃 내 핵심 의사결정 지점을 식별하고 성공 궤적을 참조해 실패 궤적을 교정하는 밀집 단계별 감독 신호를 생성한다. 이를 통해 장기 GUI 태스크에서의 희소 보상 및 공로 배분(credit assignment) 문제를 해결하며, **40억 파라미터 모델로 AndroidWorld 벤치마크에서 81.0% Pass@1 성공률**을 달성해 인간 수준을 초과했다.

## 인사이트

1. **실패에서 배운다**: 실패 궤적을 버리지 않고, 성공 궤적과 비교·대조하여 어떤 행동이 실패를 유발했는지 정밀하게 식별하는 것이 핵심이다.
2. **자율 진화 루프**: RFT 기반의 데이터-모델 공진화 구조 덕분에 값비싼 수동 라벨링 없이도 에이전트가 스스로 지속 개선할 수 있다.
3. **소형 모델의 가능성**: 4B 파라미터라는 비교적 작은 모델로도 인간 수준 이상의 GUI 자동화 성능을 달성할 수 있음을 입증했다.

## 응용 가능성

1. **모바일 RPA(로봇 프로세스 자동화)**: 반복적인 앱 조작 업무(예: 주문 처리, 데이터 입력)를 사람 개입 없이 자동화하는 엔터프라이즈 솔루션에 적용할 수 있다.
2. **접근성 보조 기술**: 시각·운동 장애 사용자를 위해 음성 명령만으로 복잡한 앱 인터페이스를 대신 조작해주는 스마트폰 어시스턴트로 활용할 수 있다.

## 추출된 엔티티

- LLM Agent

## 추출된 개념

_없음_

## 원본 파일

/storage/B8AC-56F1/papers/daily/2026-03-27-UI-VoyagerASelf-EvolvingGUIAge.md

## 메모

_마이그레이션됨_


## 관련 문서

- [[sources/2026-04-03-collaborative-task-and-path-planning-for-heterogen.md]] (공통 Entity: LLM Agent)
- [[sources/2026-03-23-navtrust-benchmarking-trustworthiness-for-embodied.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-04-stop-wandering-efficient-vision-language-navigatio.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-01-dynamic-dual-granularity-skill-bank-for-agentic-rl.md]] (공통 Entity: LLM Agent)
- [[sources/2026-04-01-amigo-agentic-multi-image-grounding-oracle-benchma.md]] (공통 Entity: LLM Agent)
