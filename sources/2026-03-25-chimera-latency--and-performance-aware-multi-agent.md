# Chimera: Latency- and Performance-Aware Multi-agent Serving for Heterogeneous LLMs

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-25
**링크**: http://arxiv.org/abs/2603.22206v1

## 💡 핵심 인사이트

멀티에이전트 LLM 워크플로우에서 각 단계별로 이기종 모델을 적응적으로 할당하는 스케줄링이 동종 배포 대비 지연시간과 성능의 파레토 최적 트레이드오프를 달성할 수 있다.

## 📖 분석

## Chimera: 이기종 LLM을 위한 지연시간 및 성능 인식 멀티에이전트 서빙

멀티에이전트 애플리케이션은 복잡한 작업을 다단계 워크플로우로 실행하며, 각 단계는 LLM 호출로 구성되고 그 출력이 후속 단계의 컨텍스트가 된다. 기존 LLM 서빙 시스템은 동일한 모델 복제본을 가진 동종(homogeneous) 클러스터를 전제로 설계되었으나, Chimera는 **이기종(heterogeneous) 배포** 환경에서 서로 다른 크기와 능력의 모델들을 활용하여 지연시간과 성능 간의 세밀한 트레이드오프를 가능하게 한다.

### 핵심 문제
멀티에이전트 시스템에서 각 에이전트 단계마다 동일한 대형 모델을 사용하는 것은 비효율적이다. 어떤 단계는 소형 모델로도 충분하고, 어떤 단계는 대형 모델이 필요하다. 이기종 환경에서는 **스케줄링의 복잡성**이 크게 증가하며, 각 단계별로 어떤 모델을 할당할지 결정하는 것이 핵심 과제가 된다.

### 기존 연구와의 연결
- **[[llm-agent]]**: Chimera는 LLM 에이전트의 실제 배포 환경에서의 서빙 최적화를 다루며, 에이전트 시스템의 프로덕션 수준 운영에 필수적인 인프라 연구이다.
- **[[multi-agent-system]]**: 다중 에이전트 워크플로우의 효율적 실행을 위한 시스템 수준 솔루션으로, Paper Circle 등 멀티에이전트 연구 프레임워크의 실행 기반이 될 수 있다.
- **[[transformer]]**: 서로 다른 크기의 Transformer 기반 모델들을 하나의 서빙 클러스터에서 효율적으로 운영하는 방법론을 제시한다.

### 의의
이 연구는 멀티에이전트 LLM 시스템이 실험실을 넘어 실제 서비스 환경으로 이행하는 데 필요한 **시스템 수준의 최적화** 방향을 제시한다. 특히 비용 효율성과 응답 품질을 동시에 고려하는 스케줄링 전략은 대규모 에이전트 서비스 운영에 실질적 가치를 제공한다.

## 🔗 관련 논문

- 2026 04 09 paper circle an open source multi agent research d
- 2026 04 09 social dynamics as critical vulnerabilities that u
- 2026 04 10 tracesafe a systematic assessment of llm guardrail
- 2026 04 10 how much llm does a self revising agent actually n

## 🏷️ 엔티티

- [[entities/llm-agent.md|llm-agent]]
- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/multi-agent-system.md|multi-agent-system]]
- [[concepts/reinforcement-learning.md|reinforcement-learning]]

---
_LLM 분석으로 재생성됨_
