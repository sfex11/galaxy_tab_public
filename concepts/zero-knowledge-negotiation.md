# zero-knowledge-negotiation

**카테고리**: 프라이버시/안전
**생성일**: 2026-04-12

## 정의

자율 에이전트가 사적 선호(private preference)를 공개하지 않으면서 합의에 도달하는 협상 프로토콜. 제로지식 증명(Zero-Knowledge Proof)을 활용하여 협상 참여자의 진정성과 합리성을 수학적으로 보장한다.

## 핵심 기술

- **Groth16 zk-SNARK**: 증명 생성 ~80ms, 제약 만족 증명에 활용
- **Paillier 암호화**: feasibility pre-check용 추가 보안 계층
- **Nash bargaining**: 근사 종료 조건으로 사용

## 구분: 2인 vs 다자간

| 항목 | 2인 협상 (선행기술) | 다자간 N≥3 (확장) |
|------|---------------------|-------------------|
| 증명 내용 | 제약 만족 (p_min ≤ p ≤ p_max) | Pareto 최적성 + 개인 합리성 (IR) |
| 대상 | Utility function 가격 범위 | 다자간 합의 합리성 |
| 아키텍처 | 단일 계층 | 3계층 분리 (Proof/Negotiation/Communication) |
| 난이도 | 중간 | 높음 (NP-hard 근사) |

## 기만 불가능성

ZKP 기반 협상은 다음 공격을 수학적으로 방지:
- **거짓 범위 신고**: p_min > p_max일 수 없음 (ZKP가 증명)
- **합의 후 파기**: 증명이 온체인 기록 가능
- **사적 정보 유출**: 검증자는 증명만 보고 내용은 알 수 없음

## 관련 논문

- [[sources/2026-01-01-device-native-autonomous-agents-for-privacy-pr.md|arXiv:2601.00911 — Device-Native Autonomous Agents for Privacy-Preserving Negotiations]] (2인 협상)
- Ransomware Negotiation (arXiv:2508.15844) — ZKP 아닌 garbled circuits 사용
- Zero-Knowledge Audit for Internet of Agents (arXiv:2512.14737) — 에이전트 감사용
- AESP (arXiv:2603.00318) — AI 에이전트 경제 거래, 결제용

## 관련 개념

- [[privacy]] — 에이전트 프라이버시 보존의 핵심 수단
- [[concepts/multi-agent-system.md|multi agent system]] — 자율 에이전트 간 협상 = MA 시스템의 새로운 패턴
- [[concepts/agent-coordination.md|agent coordination]] — 협상 프로토콜 = 조율의 한 형태
- [[concepts/ai-safety.md|ai safety]] — 사적 선호 보호 + 기만 불가능한 합의
