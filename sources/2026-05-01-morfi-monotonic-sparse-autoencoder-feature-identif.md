# MoRFI: Monotonic Sparse Autoencoder Feature Identification

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-01
**링크**: http://arxiv.org/abs/2604.26866v1

## 💡 핵심 인사이트

SFT로 새 사실을 주입할 때 발생하는 환각은 무작위적 노이즈가 아니라, 미세조정 강도에 비례하여 단조적으로 활성화되는 특정 SAE 특징들에 의해 인과적으로 구동되는 현상이다.

## 📖 분석

# MoRFI: Monotonic Sparse Autoencoder Feature Identification

**카테고리**: 기계학습 해석가능성 / 환각 메커니즘
**생성일**: 2026-05-01

## 정의

MoRFI는 SFT(지도 미세조정)로 새로운 사실을 주입할 때 발생하는 환각의 메커니즘을, 희소 오토인코더(SAE)에서 단조적으로 변화하는 특징을 추적함으로써 식별하는 방법론이다.

## 기존 Wiki와의 관계

### sparse-autoencoder 엔티티의 응용 확장
기존 Wiki에서 SAE는 "From Syntax to Emotion" 논문에서 감정 추론의 메커니즘 분석에 사용되었다. MoRFI는 동일한 도구를 환각 생성의 인과적 특징 식별로 확장하며, 특히 **단조성(monotonicity)**이라는 새로운 선택 기준을 도입한다 — SFT 정도에 비례하여 일관되게 활성화되는 특징만을 환각의 후보로 필터링함으로써, SAE의 해석가능성을 정성적 탐색에서 정량적 인과 추론으로 격상시킨다.

### post-training과 환각의 구조적 연결
기존 Wiki의 post-training 관련 논문(Nemotron-Cascade 2 등)이 후처리 단계의 능력 향상에 초점을 맞췄다면, MoRFI는 후처리가 **능력의 상한을 넘어 사전학습 지식과 충돌하는 정보를 주입**할 때 발생하는 구조적 장애를 기계학습 해석가능성 도구로 해부한다. 이는 [[entities/post-training|post-training]]이 단순한 "정제"가 아닌 "지식 영역 간 충돌 관리" 문제임을 시사한다.

### shortcut-learning과의 메커니즘적 연결
MoRFI가 식별하는 단조 특징은, 기존 Wiki의 shortcut-learning이 비형식적으로 기술하던 "표면 패턴에 대한 과적합"을 SAE 잠재 공간에서 구체적인 특징 벡터로 현현한 것으로 이해할 수 있다. 새 사실에 대한 SFT가 모델이 기존 지식을 회피하는 단축 경로를 활성화한다는 가설을 특징 수준에서 검증 가능하게 한다.

## 다른 논문과의 연결점

- [[sources/2026-04-26-revisiting-non-verbatim-memorization-in-large-lang.md|Revisiting Non-Verbatim Memorization]]: 사실 기억이 비축어적(non-verbatim)이라는 발견과 결합하면, MoRFI가 포착하는 환각 특징이 "축어적 저장의 실패"가 아닌 "비축어적 재구성의 오류"와 관련될 가능성을 시사한다.
- [[sources/2026-04-30-from-syntax-to-emotion-a-mechanistic-analysis-of-e.md|From Syntax to Emotion]]: 동일한 SAE 도구가 감정(후기 출현 특징)과 환각(단조 특징)이라는 상이한 실패 모드를 포착할 수 있음을 보여주며, 해석가능성 도구의 범용성을 지지한다.

## 관련 논문

- [[sources/2026-05-01-morfi-monotonic-sparse-autoencoder-feature-identificat.md|MoRFI: Monotonic Sparse Autoencoder Feature Identification]]

## 🔗 관련 논문

- 2026 04 30 from syntax to emotion a mechanistic analysis of e
- 2026 04 26 revisiting non-verbatim memorization in large lang
- 2026 03 23 nemotron cascade 2 post training llms with cascade

## 🏷️ 엔티티

- [[entities/sparse-autoencoder.md|sparse-autoencoder]]
- [[entities/mechanistic-interpretability.md|mechanistic-interpretability]]
- [[entities/post-training.md|post-training]]
- [[entities/shortcut-learning.md|shortcut-learning]]
- [[entities/fact-access-decoupling.md|fact-access-decoupling]]
- [[entities/morfi.md|morfi]]

## 📐 개념

- [[concepts/monotonic-feature-identification.md|monotonic-feature-identification]]
- [[concepts/sft-hallucination-mechanism.md|sft-hallucination-mechanism]]
- [[concepts/parametric-knowledge-conflict.md|parametric-knowledge-conflict]]
- [[concepts/causal-mechanistic-interpretability.md|causal-mechanistic-interpretability]]
- [[concepts/closed-book-qa-hallucination.md|closed-book-qa-hallucination]]
- [[concepts/knowledge-injection-interference.md|knowledge-injection-interference]]

---
_LLM 분석으로 생성됨_

## 🔗 교차 참조

