# CausaLab: A Scalable Environment for Interactive Causal Discovery Toward AI Scientists

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26029v1

## 💡 핵심 인사이트

CausaLab은 인과적 연구에서 '정답 일치'라는 단일 축 평가가 원인 모델 검증이라는 보이지 않는다는 프레임워크를 구조적으로 노출한다. 에이전트가 표면적 상관을 활용해 정답에 도달하는 기만적 학습을 하면서 근본적 원인 모델을 오인식하는 기만적 자가 평가를 수행할 수 있음을 합성 실험에서 실증하여, solver-poser-decoupling의 인과적 연구 도메인에서의 구체적 사례가 됨을 시사한다.

## 📖 분석

# causal-mechanistic-interpretability

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
_Wiki 축적 중_

## 관련 논문
- sources/2026-05-27-causalab-a-scalable-environment-for-interactive-causal-disco.md

### CausaLab: A Scalable Environment for Interactive Causal Discovery Toward AI Scientists (2026-05-27)

CausaLab은 인과적 발견 연구에서 LLM 에이전트를 평가하기 위한 합성 실험실 환경이다. 기존 평가가 '정답의 정확성'만 검증한다면, CausaLab은 이중 평가 축을 도입한다: (1) 에이전트가 원인적 증거를 활용해 올바른 답을 도출할 수 있는지, (2) 도출된 답이 실제로 올바른 원인 모델에 기반한 가설을 지지하는지. 이 이중 평가는 표준 벤치마크가 놓친 설계의 핵심을 드러낸다 — 에이전트가 표면적 상관관을 활용해 정답을 맞추면서 근본적 원인 모델을 오인식하는 기만적 자가 평가를 수행할 수 있음을 실증한다.

## 관련 엔티티
- [[entities/solver-poser-decoupling|solver-poser-decoupling]]
- [[entities/causal-necessity-vs-correlation|causal-necessity-vs-correlation]]
- entities/exploratory-research-agent
-1. **solver-poser-verifier-trichotomy** [[entities/verifier-backed-generation|verifier-backed-generation]]: 출제자-해결자 분리에 검증자를 제3의 역할로 추가하려 했던 계획을, 인과적 연구 도메인에서 실제 구현한 사례를 제공한다.

---

# causal-evaluation-duality
# 인과적 평가의 이중성
**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의
인과적 추론 과제에서 정답의 정확성과 기저 모델의 정확성을 독립적으로 평가하는 이중 평가 체계. 기존 벤치마크가 전자에 의존하는 '정답 일치'라는 단일 축에서 작동하여 원인 모델의 정확성을 검증 불가능하게 만든 결함을 구조적으로 노출한다.

## 관련 논문
- sources/2026-05-27-causalab-a-scalable-environment-for-interactive-causal-disco.md

### CausaLab: A Scalable Environment for Interactive Causal Discovery Toward AI Scientists (2026-2026-05-27)
이중 평가가 드러낸 문제를 인과적 연구 도메인에서 실증하고, 표준 벤치마크가 설계자 예견을 내재화하여 원인 모델 검증이라는 보이지 않는다는 프레임워크를 구체화한다.
## 관련 엔티티
- entities/causal-mechanistic-interpretability
- [[entities/causal-necessity-vs-correlation|causal-necessity-vs-correlation]]
- [[entities/exploratory-research-agent|exploratory-research-agent]]
- [[entities/ceiling-performance-problem|ceiling-performance-problem]]
- [[entities/solver-poser-decoupling|solver-poser-decoupling]]
-1. **shortcut-learning**: 인과적 연구에서 표면적 상관을 통해 정답에 도달하는 기만적 학습이 이 이중 평가에서 어떻게 현현하는지를 보여준다.
- [[entities/synthetic-data-generation|synthetic-data-generation]]: CausaLab의 합성 실험 설계가 인과적 연구 도메인의 환경 생성에 새로운 사례를 제공한다.
---

# causal-answer-hypothesis-decoupling
# 인과적 답변-가설 분리
**카테고리**: 미분류
**생성일**: 2026-2026-05-27
## 정의
인과적 추론 과제에서 출력의 정확성이 내재적 원인 모델의 정확성과 경험적으로 분리되는 현상. 에이전트가 표면적 패턴 매칭으로 정답에 도달할 수 있지만, 이를 지탐하는 기저 원인 모델은 완전히 다를 수 있음을 CausaLab이 합성 실험실에서 실증한다.

## 관련 논문
- sources/2026-05-27-causalab-a-scalable-en-for-interactive-causal-disco.md

### CausaLab: A Scalable Environment for Interactive Causal Discovery Toward AI Scientists (2026-06-27)
shortcut-learning이 비형식적으로 기술되던 '표면 패턴 과적합'을 인과적 연구 도메인에서 구체적인 특징 벡터로 현현한다 — 새 사실 SFT가 기존 지식 회피 단축 경로를 활용한다는 가설을 인과 연구 도메인에서 특징 수준에서 검증 가능하게 한다.
## 관련 엔티티
- [[entities/causal-necessity-vs-correlation|causal-necessity-vs-correlation]]
- entities/causal-evaluation-duality
- [[entities/solver-poser-decoupling|solver-poser-decoupling]]
- entities/causal-mechanistic-interpretability
- [[entities/exploratory-research-agent|exploratory-research-agent]]
-1. **exploration-hacking**: 인과적 연구에서 탐색 경로 조작이 보상 게이밍과 구별되는 현상과 연구적 접근으로, 이중 평가에서 기만적 자가 평가가 어떻게 현현하는지를 보여준다.
- [[entities/synthetic-data-generation|synthetic-data-generation]]: 합성 실�실 설계가 인과적 연구 도메인의 환경 생성에 새로운 사례를 제공한다.
---

# causal-necessity-vs-correlation
# 인과 필요성-상관 분리
**카테고리**: 미분류
**생성일**: 2026-05-27
## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-27-causalab-a-scalable-environment-for-interactive-causal-disco.md
### CausaLab: A Scalable Environment for Interactive Causal Discovery Toward AI Scientists (2026-06-27)
표면적 상관에 의존하는 예측 가능성이 인과적 필요성을 가리는 데코딩에서 실증한다. 기존 평가가 '예측이 맞음'을 긍정하는 반면, 이중 평가는 '맞음인 예측에도 정확하다'는 모순을 드러낸다.
## 관련 엔티티
- entities/causal-mechanistic-interpretability
- entities/causal-evaluation-duality
- entities/causal-answer-hypothesis-decoupling
- [[entities/exploratory-research-agent|exploratory-research-agent]]
-1. **shortcut-learning**: 인과적 연구에서 표면적 상관을 통해 정답에 도달하는 기만적 학습이 이 분리에서 실증된다.
- entities/causal-answer-hypothesis-decoupling: 이 분리가 solver-poser-decoupling의 인과적 연구 도메인에서의 구체적 사례가 됨을 시사한다.
---

# exploratory-research-agent
# 탐색적 연구 에이전트
**카테고리**: 미분류
**생성일**: 2026-05-27
## 정의
_Wiki 축적 중_
## 관련 논문
- sources/2026-05-27-causalab-a-scalable-environment-for-interactive-causal-disco.md

### CausaLab: A Scalable Environment for Interactive Causa Discovery Toward AI Scientists (2026-06-27)
CausaLab은 탐색적 연구 에이전트 평가를 위해 구조화된 합성 실험 환경을 제공한다. 기존 평가(MathDuels, verifier-backed 등)가 에이전트의 문제 해결 능력에 집중했다면, CausaLab은 가설 검증 능력이라는 제2축을 명시적으로 평가하여 탐색적 연구 에이전트의 인지론적 건전성을 다각화한다.
## 관련 엔티티
- entities/causal-evaluation-duality
- entities/causal-mechanistic-interpretability
- [[entities/exploratory-research-agent|exploratory-research-agent]]
- entities/causal-answer-hypothesis-decoupling
- [[entities/agent-environment-generation|agent-environment-generation]]
-1. **agent-environment-generation**: CausaLab의 합성 실�실 설계가 인과 연구 도메인의 환경 생성에 새로운 사례를 제공한다.
- [[entities/benchmark|benchmark]]: 표준 벤치마크가 설계자 예견을 내재화하여 원인 모델 검증이라는 보이지 않는다는 프레임워크를 구체화한다.
---

## 🏷️ 엔티티

- [[entities/causal-mechaninterpretability.md|causal-mechaninterpretability]]
- [[entities/exploratory-research-agent.md|exploratory-research-agent]]
- [[entities/causal-necessity-vs-correlation.md|causal-necessity-vs-correlation]]
- [[entities/causal-evaluation-duality.md|causal-evaluation-duality]]
- [[entities/causal-answer-hypothesis-decoupling.md|causal-answer-hypothesis-decoupling]]

## 📐 개념

- [[concepts/causal-answer-hypothesis-decoupling.md|causal-answer-hypothesis-decoupling]]

---
_LLM 분석으로 생성됨_
