# 특허 질문 1: 다자간-zkp-합리성

**날짜**: 2026-04-18
**출처**: 특허 명세서 v2 핵심 과제

## 질문
N≥3의 다수 에이전트가 각자의 사적 효용 함수를 공개하지 않으면서, 모든 참여자의 개인 합리성(Individual Rationality)을 만족하는 합의에 도달할 수 있는가? Wiki에 이와 관련된 논문이나 개념이 있는가?

## Wiki 답변

## 답변: N≥3 에이전트의 사적 효용 비공개 합의 도달 가능성

### 1. Wiki 내 직접 관련 논문 및 개념

Wiki에는 이 질문에 **정확히 일치하는 단일 논문은 없지만**, 여러 논문과 개념이 부분적으로 관련되며, 이를 결합하면 특허 출원에 유리한 구조를 도출할 수 있습니다.

#### (1) 차등 프라이버시 + 에이전트 시스템
- **[[concepts/differential-privacy.md|differential privacy]]** 엔티티 및 관련 논문 "Differential Privacy in Generative AI Agents"는 AI 에이전트 환경에서의 프라이버시 보장 메커니즘을 다룹니다. 사적 효용 함수를 공개하지 않는다는 요구사항은 차등 프라이버시(DP)로 형식화할 수 있습니다.

#### (2) 다중 에이전트 시스템의 조율
- **[[concepts/multi-agent-system.md|multi agent system]]** (16편): "다중 에이전트 조율과 다목적 트레이드오프를 동시에 해결하는 조건부 신경 솔버"(**CAMOA**)가 핵심입니다. 이 논문은 **다중 에이전트·다목적 설정에서의 최적화**를 신경망 기반으로 해결하지만, 사적 효용의 비공개는 다루지 않습니다.
- "다중 AI 에이전트 시스템에서 지연된 피드백은 인간 감독자의 오류 귀인을 체계적으로 왜곡"한다는 발견은 합의 과정의 투명성 설계와 연결됩니다.

#### (3) 에이전틱 연합학습
- **[[concepts/agent-coordination.md|agent coordination]]** 내 "Agentic Federated Learning: The Future of Distributed Training"은 분산 환경에서 로컬 데이터(=사적 정보)를 공유하지 않으면서 글로벌 모델에 합의하는 구조를 제시합니다. **연합학습의 프라이버시 보존 집계(aggregation)**는 사적 효용 비공개 합의의 기술적 선례입니다.

#### (4) 적응적 망각과 구조적 메모리
- **[[concepts/adaptive-forgetting.md|adaptive forgetting]]** 관련 논문 "Novel Memory Forgetting Techniques for Autonomous AI Agents" 및 "Coupled Control, Structured Memory, and Verifiable Action"은 에이전트가 자신의 내부 상태를 선택적으로 관리하면서도 검증 가능한 행동을 수행하는 메커니즘을 다룹니다. 이는 **효용 함수의 은닉 + 행동의 검증 가능성** 균형과 관련됩니다.

#### (5) 에이전트 아이덴티티와 신뢰
- **[[concepts/agent-identity.md|agent identity]]**: "행동 궤적만이 가장 신뢰할 수 있는 근거"라는 발견 및 "이중 불투명성"(행동 ≠ 자기 보고, 전략적 기만 가능)은 사적 효용을 공개하지 않는 에이전트 간 신뢰 구축의 근본적 난제를 명시합니다.

#### (6) 메타인지적 도구 사용
- **[[concepts/adaptive-inference.md|adaptive inference]]** 내 "Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic Models"는 에이전트가 자신의 능력과 한계를 인식하고 적절한 도구를 선택하는 메타인지를 다룹니다. 협상 과정에서 자신의 효용 경계를 인식하되 공개하지 않는 전략적 메타인지와 연결됩니다.

---

### 2. 이론적 답변

**가능합니다**, 단 조건이 필요합니다:

- **메커니즘 디자인 이론**에 의하면, Vickrey-Clarke-Groves(VCG) 메커니즘이나 Myerson-Satterthwaite 정리의 확장을 통해 사적 효용 비공개 하 개인 합리성(IR) 만족 합의가 가능합니다. 다만 N≥3에서 **예산 균형(Budget Balance)**과 **인센티브 호환성(Incentive Compatibility)**을 동시 만족하는 것은 일반적으로 불가능하므로(Myerson-Satterthwaite), **근사적 해**가 필요합니다.
- Wiki의 차등 프라이버시 + 연합학습 기반 접근은 이를 **노이즈 주입을 통한 ε-차등 프라이버시 보장 하에서의 근사적 IR 만족 합의**로 구현할 수 있는 경로를 제공합니다.

---

### 3. 특허 출원 관점의 유리한 근거

**핵심 특허성 주장: "LLM 에이전트 환경에서의 프라이버시 보존 다자간 합의 프로토콜"**

| 근거 | Wiki 출처 | 특허 적용 |
|------|-----------|-----------|
| 기존 메커니즘 디자인은 LLM 에이전트에 미적용 | [[entities/llm-agent.md|llm agent]] 97편 중 협상/합의 관련 메커니즘 디자인 부재 | **선행기술 부재 → 신규성** |
| DP가 에이전트에 적용되기 시작 | [[concepts/differential-privacy.md|differential privacy]] 논문 | DP를 효용 함수 은닉에 적용하는 것은 미개척 |
| 연합학습의 집계 구조가 선례 | Agentic Federated Learning | FL의 secure aggregation을 효용 합의로 전용 |
| 에이전트 아이덴티티의 이중 불투명성 | [[concepts/agent-identity.md|agent identity]] | 행동 궤적 기반 합의 검증 메커니즘의 필요성 |
| 검증 가능한 행동 구조 | Coupled Control, Structured Memory | 효용 비공개 + 행동 검증 가능성의 아키텍처적 해결 |

---

### 4. 기존 기술과의 차별성 분석

| 기존 기술 | 한계 | 제안 가능한 차별화 |
|-----------|------|-------------------|
| **VCG 메커니즘** | 정적, 예산 불균형, LLM 에이전트 미고려 | LLM 에이전트의 동적 추론 과정에 메커니즘 디자인 내장 |
| **Secure Multi-Party Computation (SMPC)** | 연산 비용 높음, 실시간 에이전트 상호작용에 부적합 | 경량 DP 노이즈 + LLM의 자연어 기반 협상으로 대체 |
| **연합학습** | 모델 파라미터 집계에 특화, 효용 함수 합의에 미적용 | FL의 secure aggregation을 효용 공간으로 일반화 |
| **CAMOA (Wiki 내)** | 다목적 최적화이나 사적 효용 비공개 메커니즘 없음 | 프라이버시 보존 레이어 추가 |
| **기존 LLM 협상 연구** | 효용 함수가 공개되거나 단순한 제로섬 설정 | N≥3 비제로섬, 비공개 효용, IR 보장의 조합 |

---

### 5. 특허 청구항 방향 제안

위 Wiki 분석을 종합하면, 다음과 같은 발명이 **신규성 + 진보성**을 주장할 수 있습니다:

> **"차등 프라이버시 보장 하에 N≥3 LLM 에이전트가 사적 효용 함수를 공개하지 않으면서 개인 합리성을 만족하는 합의에 도달하는 프로토콜"**

구성요소:
1. 각 에이전트가 자신의 효용 함수에 ε-DP 노이즈를 주입한 **마스킹된 선호 신호**를 생성
2. 연합학습 스타일의 **secure aggregation**으로 전체 효용 공간의 파레토 프론티어를 근사
3. **메타인지 모듈**(Act Wisely 참조)이 각 에이전트의 IR 위반 여부를 자체 검증
4. **행동 궤적 기반 감사**(agent-identity 참조)로 합의 이행을 사후 검증
5. **적응적 망각**(adaptive-forgetting 참조)으로 협상 과정의 중간 정보를 안전하게 폐기

Wiki 내에 이 조합을 정확히 구현한 선행 연구가 **존재하지 않으므로**, 특허 출원 시 신규성 주장이 유리합니다.

---
_특허 Wiki Query로 생성됨_
