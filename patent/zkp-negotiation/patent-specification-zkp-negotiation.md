# ZKP 협상 특허 — 기술 명세서 (초안)

## 1. 발명의 명칭
**프라이버시 보존 다자간 자율 협상 시스템 및 그 방법**

## 2. 기술분야
본 발명은 제로지식 증명(Zero-Knowledge Proof) 기반으로, 다수의 자율 에이전트가 자신의 사적 선호(private preference)를 공개하지 않으면서, 파레토 최적(Pareto Optimal)이고 개인 합리성(Individual Rationality)을 만족하는 합의에 도달하는 협상 시스템에 관한 것이다.

## 3. 배경기술

### 3.1 기존 기술의 한계
- **단일 검증자 모델**: 기존 LLM-as-a-judge는 단일 모델의 편향에 취약
- **2인 협상 한계**: arXiv:2601.00911은 2인 협상에서 제약 만족(p_min ≤ p ≤ p_max)만 증명
- **신원 고정**: DRC-369, FractalNode는 영구 신원(persistent identity)에 집중, 이식성(portability) 미흡
- **MIGT 분류법**: 거버넌스 택소노미 제공하나, 구현 메커니즘 미제시

### 3.2 선행기술 분석
| 선행기술 | 한계 |
|----------|------|
| arXiv:2601.00911 (2인 ZKP 협상) | N≥3 다자간 미지원, Pareto 증명 없음 |
| DRC-369 (Soulbound NFT) | 전송 불가, 단일 플랫폼 한정 |
| SPIFFE (workload identity) | 인프라 수준, 에이전트 자격 증명 미포함 |
| SMPC 일반 (4,569건) | Pareto+bargaining+privacy 조합 없음 |

## 4. 해결하려는 과제
1. N≥3 에이전트가 각자의 utility function을 공개하지 않으면서 합리적 합의에 도달하는 방법
2. 합의가 Pareto 최적임을 수학적으로 증명하면서 프라이버시를 보존하는 방법
3. 증명 크기와 검증 시간을 polynomial로 유지하면서 NP-hard 문제를 근사 증명하는 방법
4. 블록체인 없이 분산 합의 기반으로 신원 이식성(identity portability)을 보장하는 방법

## 5. 발명의 구성

### 5.1 전체 시스템 구성

```
┌─────────────────────────────────────────────────────┐
│                    PCN 3계층 아키텍처                  │
│                                                       │
│  ┌──────────┐   ┌──────────────┐   ┌──────────────┐  │
│  │ P (Proof)│──→│ C (Comm)     │──→│ N (Negotiate)│  │
│  │ 계층     │   │ 계층         │   │ 계층          │  │
│  │          │   │              │   │              │  │
│  │ Groth16  │   │ Paillier     │   │ 교대 오퍼     │  │
│  │ zk-SNARK│   │ 동형 암호     │   │ ε-Pareto     │  │
│  │          │   │              │   │ 근사 종료     │  │
│  └──────────┘   └──────────────┘   └──────────────┘  │
│                                                       │
│  에이전트 A  에이전트 B  에이전트 C  ...  에이전트 N    │
└─────────────────────────────────────────────────────┘
```

### 5.2 P계층 (Proof Layer) — 상세 명세

#### 5.2.1 개인 합리성 증명 (IR Proof)

**입력:**
- 에이전트 i의 utility function: uᵢ(x)
- 협상 불참 시 보장치: uᵢ(x₀)
- 합의안: x*

**증명 내용:**
```
π_IR_i = Groth16.Prove(
    circuit: "u_i(x*) ≥ u_i(x₀)",
    witness: (u_i, x*, x₀),
    public_input: (commitment_i, hash(x*), hash(x₀))
)
```

** 증명 크기:** ~200 bytes (Groth16 고정)
** 증명 생성 시간:** ~80ms
** 검증 시간:** ~5ms

#### 5.2.2 ε-Pareto 최적성 증명 (ε-Pareto Proof)

**정의:** 합의안 x*가 ε-Pareto 최적이란:
```
∀x ∈ X: Σᵢ uᵢ(x*) ≥ Σᵢ uᵢ(x) - ε
```

**근사 알고리즘 (핵심 혁신):**

```
Algorithm: ε-ParetoNegotiate(N, ε, δ)
Input: N명 에이전트, 근사 오차 ε > 0, 실패 확률 δ
Output: 합의안 x*, 증명 π_pareto

1. 각 에이전트 i가 commitment_i = Commit(uᵢ) 생성 → C계층으로 전송
2. 메디에이터 없이 교대 오퍼 진행:
   a. 무작위 순서로 에이전트 선택 (round-robin)
   b. 각 에이전트가 암호화된 counter-offer 제안
   c. Paillier 덧셈 동형성으로 총 utility 합산 (개별 값 노출 없이)
3. 수렴 조건:
   Σ_encrypted_u ≥ Σ_baseline - ε 이면 합의 선언
4. 증명 생성:
   π_pareto = Groth16.Prove(
       circuit: "Σ u_i(x*) ≥ max_x Σ u_i(x) - ε",
       witness: (Σ u_i, ε, x*),
       public_input: (Σ_commitments, hash(x*), ε)
   )
```

**복잡도 분석:**
| 항목 | 복잡도 |
|------|--------|
| 통신 라운드 | O(N log N) |
| 증명 크기 | O(1) — Groth16 고정 |
| 검증 시간 | O(1) |
| 총 연산량 | O(N² log N) — NP-hard 근사 |

### 5.3 C계층 (Communication Layer) — 상세 명세

#### 5.3.1 Paillier 동형 암호 프로토콜

**키 생성:**
```
p, q: 큰 소수
n = p × q
g = n + 1
공개키: (n, g)
비밀키: (p, q)
```

**암호화:**
```
E(m) = g^m × r^n mod n²    (r: 무작위)
```

**덧셈 동형성 (핵심):**
```
E(m₁) × E(m₂) = E(m₁ + m₂) mod n²
```

이를 활용하여 각 에이전트의 utility를 암호화한 상태로 합산 가능:
```
E_total = Πᵢ E(uᵢ(x*)) = E(Σᵢ uᵢ(x*))
```

**Feasibility Pre-check:**
```
1. 각 에이전트가 E(uᵢ(x₀)) 전송 (불참 시 보장치)
2. E_total_threshold = Πᵢ E(uᵢ(x₀)) = E(Σᵢ uᵢ(x₀))
3. 협상 중 E_total_current와 비교
4. E_total_current ≥ E_total_threshold이면 IR 만족 가능
```

#### 5.3.2 메시지 규격

```
Message Format:
┌────────────────────────────────────────┐
│ type: OFFER | ACCEPT | REJECT | PROOF │
│ sender_id: agent_id                    │
│ round: uint32                           │
│ payload: Paillier_ciphertext            │
│ proof: Groth16_proof (optional)        │
│ signature: Ed25519                     │
└────────────────────────────────────────┘
```

### 5.4 N계층 (Negotiation Layer) — 상세 명세

#### 5.4.1 교대 오퍼 프로토콜

```
Protocol: AlternatingOffer(N, ε)
State: (round, current_proposal, accept_count)

INIT:
  round = 0
  current_proposal = null
  accept_count = 0

LOOP:
  1. round++
  2. proposer = agents[round mod N]
  3. proposer가 Paillier 암호화된 counter-offer 전송
  4. C계층을 통해 E_total_current 계산 (암호화 상태)
  5. IF E_total_current ≥ E_total_threshold:
       a. 모든 에이전트에게 accept 요청 전송
       b. 각 에이전트가 IR 증명(π_IR_i) 생성 → P계층
       c. accept_count 증가
       d. IF accept_count == N:
            합의 성립 → Pareto 증명 생성 → 종료
  6. IF round > MAX_ROUNDS:
       협상 실패 → ε 증가 후 재시도 또는 중단
```

#### 5.4.2 수렴 보장

**정리:** ε > 0인 경우, 다자간 협상은 유한 라운드 내에 수렴한다.

**증명 스케치:**
- Nash Bargaining Solution(NBS)은 Pareto 최적임이 수학적으로 보장
- ε-근사로 NBS에 충분히 가까운 해가 존재
- 교대 오퍼는 monotonically improving
- 따라서 유한 라운드 내 ε-근사 도달

## 6. 실시예 (Embodiments)

### 실시예 1: 3인 보험 협상
- 3개 보험사 에이전트가 리스크 분담 협상
- 각자의 한계 수용력(acceptance capacity)을 공개하지 않음
- 합의안이 Pareto 최적 + 모든 참여자가 현재 단독 처리보다 유리함을 ZKP로 증명

### 실시예 2: N인 클라우드 리소스 분배
- N개 테넌트가 클라우드 리소스 분배 협상
- 각자의 예산과 수요를 공개하지 않음
- ZKP로 합리성 증명 + Paillier로 총 수요 합산

### 실시예 3: 크로스 플랫폼 신원 이식
- 에이전트가 플랫폼 A에서 플랫폼 B로 이동
- A에서의 자격/평판을 공개하지 않으면서 B에서 유효성 증명
- ZKP로 "이 에이전트는 A에서 충분한 자격을 갖춤"만 증명

## 7. 청구항 (Claims) — 초안

### 독립항 1
다수의 자율 에이전트가 각자의 사적 선호 정보를 공개하지 않으면서 협상에 참여하는 프라이버시 보존 다자간 협상 방법에 있어서,
(a) 각 에이전트가 자신의 효용 함수에 대한 커밋먼트를 생성하는 단계;
(b) 동형 암호 체계를 이용하여 암호화된 상태에서 교대 오퍼를 교환하는 단계;
(c) 상기 동형 암호의 덧셈 동형성을 이용하여 전체 효용 합을 암호화 상태로 계산하는 단계;
(d) 상기 합이 사전 정의된 임계값 이상인 경우, 합의를 수락하는 단계;
(e) 각 에이전트가 zk-SNARK를 이용하여 자신의 개인 합리성을 증명하는 단계;
(f) 상기 합의안의 ε-Pareto 최적성을 zk-SNARK로 증명하는 단계;
를 포함하는 것을 특징으로 하는 방법.

### 종속항 2
청구항 1에 있어서,
상기 (c) 단계에서 Paillier 암호화 체계를 사용하며,
상기 암호화된 효용 합을 복호화하지 않고 임계값과 비교하는 것을 특징으로 하는 방법.

### 종속항 3
청구항 1에 있어서,
상기 (e) 단계의 zk-SNARK가 Groth16 프로토콜을 사용하며,
증명 크기가 O(1)이고 검증 시간이 O(1)인 것을 특징으로 하는 방법.

### 종속항 4
청구항 1에 있어서,
상기 (a)~(f) 단계를 증명(Proof), 통신(Communication), 협상(Negotiation)의 3개 독립 계층으로 분리하여 수행하는 것을 특징으로 하는 방법.

### 종속항 5
청구항 1에 있어서,
참여 에이전트 수가 N≥3이며,
상기 ε-Pareto 최적성이 NP-hard 문제의 근사 해로서,
ε을 0에 수렴시킴으로써 정확한 Pareto 최적에 근사하는 것을 특징으로 하는 방법.

### 종속항 6 (Identity Portability 연계)
청구항 1에 있어서,
상기 협상의 결과로 얻은 합의안이 에이전트의 신원 이식에 사용되며,
제1 플랫폼에서의 자격을 공개하지 않으면서 제2 플랫폼에서 상기 zk-SNARK 증명을 통해 자격의 유효성을 검증하는 것을 특징으로 하는 방법.

## 8. 발명의 효과
1. N≥3 다자간 협상에서 프라이버시 완전 보존 (기존 2인 한계 극복)
2. 증명 크기 O(1), 검증 시간 O(1)로 실시간 검증 가능
3. NP-hard 문제를 ε-근사로 polynomial 시간 해결
4. 3계층 분리로 모듈식 업그레이드 가능
5. 블록체인 없이 분산 합의 기반으로 구현 가능
6. Identity Portability와 결합하여 크로스 플랫폼 자격 증명 가능
