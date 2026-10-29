# MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-10-29
**링크**: http://arxiv.org/abs/2610.37647v1

## 💡 핵심 인사이트

노름 제어의 실질 기능은 가중치 노름 자체의 관리가 아니라 누적 유효 학습률($η/\|W\|_F$의 궤적 합)이라는 단일 적분량의 관리로 환원된다.

## 📖 분석

# MuonGS: Pretraining LLMs with Relaxed Weight-Norm Control

Muon 옵티마이저의 노름 제어(norm control)를 훈련 궤적 전체에 걸쳐 **누적 유효 학습률** $C_T=\sum_{t<T}η_t/\|W_t\|_F$이라는 단일 스칼라로 분석한다. 유효 학습률은 명목 학습률을 가중치 노름으로 나눈 값으로, 노름 제어가 실제로 하는 일은 '학습률의 분모를 관리하는 것'임을 정식화한다. 기존의 weight decay·명시적 노름 제약 논의가 각 메커니즘의 경험적 효과에 머물렀다면, 본 논문은 '왜 도움이 되는가, 얼마나 필요한가'를 통일된 궤적 수준 지표로 설명한다.

## Wiki와의 연결

이 논문은 [[parameter-decoupling]]의 옵티마이저 버전이다. 해당 개념이 '품질 목표와 비용 목표가 별도 파라미터 축으로 분해 가능함'을 사후학습(LOCUS)에서 보였다면, MuonGS는 **사전학습 단계에서 표면 파라미터(가중치 노름)와 실제 제어 변수(유효 학습률)의 분리**를 보여준다. 노름 자체가 아니라 $η/\|W\|_F$가 실제 업데이트 강도를 결정하므로, 제어해야 할 대상이 파라미터 표면이 아닌 비율임을 확정한다.

또한 [[score-centering]] 계열의 '훈련 역학의 계통적 변수 식별' 흐름에 속한다. Score Centering이 훈련-추론 엔진 간 drift를 누적 편향으로 진단하고 중심화로 제거했다면, MuonGS는 사전학습에서 노름 궤적이 누적 유효 학습률로 환원됨을 보여, 훈련 안정성 연구가 **스텝 단위 직관에서 궤적 수준 적분량으로 이동**하고 있음을 강화한다.

[[transfer-learning]] 관점에서도 의미가 있다: 노름 제어의 필요량이 스케일과 궤적에 조건부라는 분석은, 사전학습→미세조정 전이에서 유효 조건 명시가 필수라는 PDE 서러게이트 연구의 정신과 공명한다.

## 🏷️ 엔티티

- [[entities/optimizer-norm-control.md|optimizer-norm-control]]
- [[entities/accumulated-effective-learning-rate.md|accumulated-effective-learning-rate]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/score-centering.md|score-centering]]

## 📐 개념

- [[concepts/effective-learning-rate.md|effective-learning-rate]]
- [[concepts/weight-norm-control.md|weight-norm-control]]
- [[concepts/training-trajectory-analysis.md|training-trajectory-analysis]]
- [[concepts/optimizer-design.md|optimizer-design]]

---
_LLM 분석으로 생성됨_
