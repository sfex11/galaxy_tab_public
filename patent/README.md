# 📋 특허 포트폴리오

> ZKP 기반 프라이버시 보존 협상 + 에이전트 신원 이식성 관련 특허 문서

---

## 📁 구조

### [ZKP 협상 특허](zkp-negotiation/) — 1순위 (등록 확률 80-85%)

| 파일 | 설명 |
|------|------|
| [patent-specification-final.md](zkp-negotiation/patent-specification-final.md) | **명세서 완성본** — 청구항 8개, 실시예 3개, 요약서 |
| [patent-specification-zkp-negotiation.md](zkp-negotiation/patent-specification-zkp-negotiation.md) | 기초 초안 |
| [diagrams.html](zkp-negotiation/diagrams.html) | **도면 5장** — 시스템 구성도, 흐름도, 시퀀스, 신원이식, DRC-369 대비 |
| [patent_poc_zkp_negotiation.py](zkp-negotiation/patent_poc_zkp_negotiation.py) | **PoC 코드** — Paillier + ZKP 시뮬레이션 |

### [Identity Portability 특허](identity-portability/) — 3순위 (준비 중)

> DRC-369 대응 차별화 전략 수립 완료. 상세 설계 진행 예정.

### [출원 로드맵](roadmap.html)

Phase 1~6 전체 진행 상황

---

## 📊 현재 상태

| Phase | 내용 | 상태 |
|-------|------|------|
| 1 | 기술 명세서 | ✅ 완료 |
| 2 | 도면 5장 | ✅ 완료 |
| 3 | PoC 구현 | ✅ 완료 |
| 4 | 명세서 완성본 | ✅ 완료 |
| 5 | 변리사 검토 → 출원 | ⏳ 대기 |
| 6 | Identity Portability | ⏳ 대기 |

---

## 🔑 핵심 청구항 요약

**독립항 1:** 6단계 방법 — 커밋먼트 → Paillier 동형 오퍼 → 암호화 합산 → 수렴 판정 → Groth16 IR 증명 → ε-Pareto 증명

**청구항 6:** 크로스 플랫폼 신원 이식 — 제1 플랫폼 자격을 공개하지 않고 제2 플랫폼에서 ZKP 검증

**청구항 8:** 컴퓨터 기록 매체

---

## 📚 관련 블로그

- [Identity Portability + ZKP 최종 조사](../blog/identity-portability-zkp-final-survey.html)
- [ZKP 심화 분석](../blog/zkp-patent-deep-dive.html)
- [ZKP 특허 분석](../blog/zkp-patent-analysis.html)

---

*최종 업데이트: 2026-04-12*
