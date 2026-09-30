# Late Attention Layers Alone Can Copy Entity Tokens, but Not Without Attending to Their Context

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-30
**링크**: http://arxiv.org/abs/2609.35663v1

## 💡 핵심 인사이트

LLM의 개체 토큰 복사는 후기 어텐션 계층의 단독 능력이 아니라 맥락 토큰 어텐션을 전제로 한 계층 간 분업이며, 개체 접근은 원자적 연산이 아니라 맥락 조건부의 관계적 연산이다.

## 📖 분석

본 논문은 LLM의 개체 복사(entity copying) — 프롬프트 속 개체를 지칭하는 토큰(entity token)을 출력으로 옮기는 기본 기능 — 에 대해 최초의 체계적 계층별 설명을 제공한다. 핵심 발견은 이중 구조다: 후기 어텐션 계층만으로 개체 토큰 복사가 가능하지만, 동일 시퀀스의 맥락 토큰(context token)에 대한 어텐션이 없으면 복사가 실패한다. 즉 복사는 원자적 패턴 매칭이 아니라, 선행 계층의 맥락 통합이 전제된 계층 간 분업으로 실현된다.

Wiki와의 연결: [[fact-access-decoupling]]이 다룬 '사실 저장-사실 접근 분리'에 기계론적 근거를 부여한다 — 개체 토큰 접근이 독립 연산이 아니라 맥락 조건부임을 층 수준에서 실증한다. [[entity-surface-form]]의 verbatim/non-verbatim 기억 감사에 '컨텍스트 내 복사'라는 대응 축을 제공하여, 개체 표면형이 맥락 토큰과 결합된 상태로만 처리됨을 기제 수준에서 확인시킨다. [[causal-head-level-attribution]]의 Deep Noir 계열 판독 패러다임에 '기능별 계층 전문화'라는 새 분석 대상을 추가하며, [[in-context-learning]]의 복사 프리미티브를 분해한다. [[attention-sink]]·[[attention-self-concentration]] 계열의 어텐션 분포 구조 연구와 함께, 어텐션 배분이 기능 실현의 기판임을 강화한다.

## 🔗 관련 논문

- It's Not RoPE that Creates Sinks: The Role of Self-Concentra
- Deep Noir: Autonomous Steering Discovery via Architectural C

## 🏷️ 엔티티

- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/fact-access-decoupling.md|fact-access-decoupling]]
- [[entities/entity-surface-form.md|entity-surface-form]]
- [[entities/causal-head-level-attribution.md|causal-head-level-attribution]]
- [[entities/in-context-learning.md|in-context-learning]]
- [[entities/entity-token-copying.md|entity-token-copying]]

## 📐 개념

- [[concepts/entity-token-copying.md|entity-token-copying]]
- [[concepts/context-dependent-copying.md|context-dependent-copying]]
- [[concepts/layer-wise-functional-specialization.md|layer-wise-functional-specialization]]

---
_LLM 분석으로 생성됨_
