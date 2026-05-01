# DV-World: Benchmarking Data Visualization Agents in Real-World Scenarios

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-04-30
**링크**: http://arxiv.org/abs/2604.25914v1

## 💡 핵심 인사이트

벤치마크의 구조적 한계(샌드박스 격리·단일 언어·완전 의도 가정)가 도메인 무관하게 에이전트의 실제 능력을 과대평가하며, 이를 해결하려면 평가 환경 자체가 아닌 평가의 존재론적 전제(환경·언어·의도)를 먼저 교정해야 한다.

## 📖 분석

# DV-World: Benchmarking Data Visualization Agents in Real-World Scenarios

## 정의
데이터 시각화(DV) 에이전트를 실제 프로페셔널 라이프사이클 전반에서 평가하는 260개 태스크 기반 벤치마크. 기존 벤치마크의 세 가지 구조적 한계를 진단하고 이를 극복한다.

## 기존 Wiki와의 관계

### sandbox-liveworld-gap의 DV 도메인 인스턴스
DV-World는 기존 벤치마크가 코드 샌드박스에 에이전트를 가둬 평가한다는 점을 'code-sandbox confinement'으로 명명하며, 이것이 [[concepts/sandbox-liveworld-gap|샌드박스-실세계 격차]]의 DV 도메인 특화 현현임을 보여준다. ClawBench가 웹 태스크에서 65-75%→33.3%로 급락한 패턴과 동일한 구조가 DV에서도 존재할 가능성을 제기한다.

### evaluator-assumption의 구체화
'assumption of perfect intent'이라는 용어로 기존 [[entities/evaluator-assumption|평가자의 가정]]을 DV 도메인에서 구체화한다. 사용자 의도가 완전히 주어진다는 가정이 실제 프로페셔널 워크플로우에서는 성립하지 않으며, 이 가정이 측정하는 것이 에이전트 능력이 아니라 가정의 부산물임을 보인다.

### computer-use-agent의 능력 확장
DV 에이전트는 [[entities/computer-use-agent|컴퓨터 사용 에이전트]]의 하위 유형으로, 시트 조작(Sheet), 크로스 플랫폼 진화, 의도 정렬이라는 세 가지 추가 능력 차원을 제공한다.

## 연결점
- [[sources/2026-04-23-chat2workflow-a-benchmark-for-generating-executabl.md|Chat2Workflow]]와 함께 시각적 워크플로우 생성/평가 축을 형성하되, Chat2Workflow가 생성에 집중한다면 DV-World는 전체 라이프사이클(생성→수정→진화)을 아우른다는 차이가 있다.
- [[entities/swe-chat|SWE-chat]]이 코딩 에이전트의 야생 환경 데이터를 제공한 것과 유사하게, DV-World는 DV 에이전트의 실제 프로페셔널 환경 평가 경로를 연다.

## 🔗 관련 논문

- 2026 04 23 chat2workflow a benchmark for generating executab
- 2026 04 24 swe chat coding agent interactions from real users
- 2026 04 29 defective task descriptions in llm based code gene

## 🏷️ 엔티티

- [[entities/dv-world.md|dv-world]]
- [[entities/dv-agent.md|dv-agent]]
- [[entities/computer-use-agent.md|computer-use-agent]]
- [[entities/benchmark.md|benchmark]]
- [[entities/evaluator-assumption.md|evaluator-assumption]]

## 📐 개념

- [[concepts/code-sandbox-confinement.md|code-sandbox-confinement]]
- [[concepts/proactive-intent-alignment.md|proactive-intent-alignment]]
- [[concepts/cross-platform-evolution.md|cross-platform-evolution]]
- [[concepts/native-environmental-grounding.md|native-environmental-grounding]]
- [[concepts/professional-lifecycle-evaluation.md|professional-lifecycle-evaluation]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

- → [[sources/2026-04-30-restestbench-a-benchmark-for-evaluating-the-effect]]: 두 논문 모두 특정 도메인(데이터 시각화, REST API 테스트)에서 기존 벤치마크가 지닌 구조적 한계(샌드박스 격리, 무감각한 메트릭)를 지적하고, 실제 실무 환경의 복잡성을 반영한 새로운 평가 체계를 제안한다.
