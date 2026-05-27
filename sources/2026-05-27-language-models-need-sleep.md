# Language Models Need Sleep

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26099v1

## 💡 핵심 인사이트

기존 KV 캐시 최적화 연구가 '캐시에 더 많이 담는 방향'의 트레이드오프를 다루는 반면, sleep-wake는 그 역방향—'컨텍스트를 압축하여 모델로 보존'—으로 패러다임을 제안한다. 이 전환은 KV 캐시의 물리적 한계가 아니라 모델 수용의 구조적 한계임을 근본적으로 해소하며, long-context의 근본적 한계를 longseeker과 대척점을 형성한다.

## 📖 분석

# Sleep-Wake Consolidation: 주기억의 압축적 전이

기존의 KV 캐시 최적화 연구(압축, 양자화, KV cache 양자화 등)가 '캐시를 더 효율적으로 저장'하는 방향의 연구를 반전시킨다. 이 논문은 반대로 **주기억의 의미론을 압축하여 가중치를 모델 파라미터로 전이**시키는 패러다임을 제안한다. 에이전트가 최근 컨텍스트를 State Space Model (SSM) 블록의 빠른 가중치 업데이트를 통해 영속화(fast weight)시키고, 이후 KV 캐시를 초기화하여 새 컨텍스트를 위한 공간을 확보하는 '수면-수면 주기 체제(Sleep-Wake)'를 제안한다.

기존 KV 캐시 연구가 '저장 용량과 추론 품질의 비선형 트레이드오프'를 다루는 반면, 이 접근은 그 트레이드오프를 **구조적으로 해결**한다. 컨텍스트 길이를 무한히 확장하는 것이 아니라, 주기적으로 중요한 정보를 주기적으로 SSM 블록에 압축한 뒤 **전체 컨텍스트를 의미론적 잔존으로 변환**하여 KV 캐시의 물리적 한계를 극복한다. 이는 [[kv-cache-optimization]]이 다루는 압축-양자화 접근(캐시 압축, 양자화, KV 양자화 등이 모두 '캐시 용량을 늘리는 방향'이라는 공통 전제를 공유하지만, 해결 방향이 정반대인 점에서 출발한다는 구조적 대안이다.

kv-cache-optimization: 캐시 길이에 비례례적으로 증가하는 스펙샷으로, 기존 연구는 KV 캐시의 물리적 한계와 추론 비용의 비선형 트레이드오프를 동시에 해결하지 못한다. 압축 기반 접근(TeCoD 등)과 달리, 외부 검증이 필요 없는 의미론적 보존을 보장한다는 점에서 기존 연구의 한계를 구조적으로 해소한다.

long-context: Transformer의 어텐션 메커니즘이 컨텍스트 길이에 따라 비선형적으로 악화되어, 긴 컨텍스트에서 추론 품질이 저하되는 근본적 한계를 다룬다. 이 논문은 주기적 압축이 컨텍스트 길이 무한하더라도 SSM 블록의 수용 capacity 내에서 추론 품질을 보존할 수 있게 하여, [[long-context]]의 근본적 한계를 구조적으로 해소한다.

memory-management: 메모리 관리 연구(적응적 망각, FORGE 등)가 저장 효율과 재사용 사이의 근본적 한계를 다루나 반면, sleep-wake는 망각이 메모리 인프라가 아닌 모델 파라미터 자체를 메모리로 활용하여 **모델 재훈련 없이 외부 경험을 내재화**하는 새로운 메모리 패러다임을 제안한다. continual-learning 연구의 외부 인프라(파이프라인, FORGE) 의존성을 보완하여, 메모리 충돌 실패와 memory-fragmentation-failure 문제를 회피하는 경로를 제공한다.

episodic-context: 에피소딕 컨텍스트가 단기적 기억으로만 기능하는 것이 아니라, sleep-wake를 통해 **영구적(semantic) 메모리로 변환**됨을 보여준다. 이는 episodic-context의 '_Wiki 축적 중_' 상태를 구체화한다.

persistent-world-model: DeltaBox가 체크포인트 롤백으로 상태를 보존하려는 반면, sleep-wake는 모델 가중치에 지식을 **비�러적(non-volatile)으로 영구화**한다. 체크포인트 롤백이 '상태를 어디까지 복원하는가'를 다루는 반면, sleep-wake는 '상태를 어떻게 보존하는가'를 근본적으로 해결한다. delta-checkpoint-rollback와 대조됨다.

agent-os-semantic-gap: 에이전트의 의미론적 의존 그래프를 OS 수준의 체크포인트 메커니즘이 번역할 때 발생하는 의미론 보존 실패를, 모델 가중치 업데이트 자체가 의미론적 보존을 달성함으로써, algorithm-system-translation-gap을 가중치 수준에서 해소한다. crab의 의미론 인식 C/R이 개별 에이전트 수준에서는 실행 환경 계층의 문제로 남는 것과 대조된다.

## 🏷️ 엔티티

- [[entities/sleep-wake-consolidation.md|sleep-wake-consolidation]]

## 📐 개념

- [[concepts/context-consolidation.md|context-consolidation]]

---
_LLM 분석으로 생성됨_
