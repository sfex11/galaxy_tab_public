# knowledge-distillation

**카테고리**: 미분류
**생성일**: 2026-05-01

## 정의

_Wiki 축적 중_

## 관련 논문

- [[sources/2026-05-01-select-to-think-unlocking-slm-potential-with-local.md|Select to Think: Unlocking SLM Potential with Local Sufficie]]

### Turning the TIDE: Cross-Architecture Distillation for Diffusion Large  (2026-05-01)

동일 아키텍처 내 파라미터 축소에 머물던 기존 정의를 '아키텍처·어텐션 메커니즘·토크나이저가 상이한 모델 간 지식 전이'로 확장하며, 지식 증류의 근본적 전제인 '표현 공간의 동일성' 가정을 해체하는 첫 실증 사례를 제공한다.

### Standing on the Shoulders of Giants: Stabilized Knowledge Distillation (2026-05-05)

증류의 목표를 '능력 전이'에서 '안정성 전이'로 확장하는 실증을 제공한다. 소형 모델이 의미론적 판단은 가능하나 구조화된 출력 생성과 추론 지시 준수에서 불안정하다는 현상을 문제화하고, 증류 타겟에 출력 형식 준수를 명시적으로 포함하여 이를 해결한다. 기존 정의가 '무엇을 알게 하는가'에 집중했다면, 본 논문은 '어떻게 안정적으로 표현하게 하는가'라는 동등하게 중요한 차원을 추가한다.

### Standing on the Shoulders of Giants: Stabilized Knowledge Distillation (2026-05-06)

지식 증류의 병목을 '용량 전이'에서 '형식 준수 전이'로 확장한다. 기존 TIDE가 아키텍처 간 표현 공간 불일치를 다루고 Select to Think가 SLM 내재 능력의 동적 활성화를 다루었다면, 본 논문은 규모 간 형식 준수성이라는 제3의 병목 축을 식별하여 지식 증류의 적용 전제를 구조적으로 재검토하게 한다.

### Distill Globally, Adapt Locally: Reasoning Distillation and Product-Ty (2026-09-08)

증류의 종착점을 언어 모델에서 벗어나 비생성적 판별 모델로 확장한다 — 전이되는 것이 토큰 분포가 아니라 '무엇이 업그레이드이고 무엇이 의도 이탈인가'라는 판단 기준임을 보여, TIDE(아키텍처 간 전이)·안정화 KD(형식 안정성 전이)와 함께 증류의 스펙트럼에 '추론→결정 논리 전이'라는 새 축을 추가한다.

### Discrete Beckmann Transport Models for One-Step Language Modeling and  (2026-09-16)

증류의 품질 상한 문제가 스텝 압축 도메인에서 어떻게 발현되는지 규명한다 — 교사의 다단계 분포만 학습 가능한 학생의 원스텝 생성은 구조적으로 교사 품질 이하로 갇히며, DBTM은 생성 목표를 직접 훈련해 이 종속성을 제거한다.

### Merging the Knowledge of LLMs for Automatic Speech Recognition (2026-09-16)

증류(교사 출력 모방)와 병합(가중치 직접 결합)이 외부 지식 통합의 별개 경로임을 대비시킨다. 교사 모델의 런타임 추론 없이도 텍스트 전용 LM의 지식이 음성 모델로 이전 가능함을 시사한다.

### StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks vi (2026-09-19)

증류의 원료가 지식(로짓)이 아니라 판단 행위 자체임을 보여준다 — VLM의 전이 판단 궤적이 증류 데이터가 되는 agentic distillation이라는 새 변형이다.

### StageGuard: Learning Stage Transitions for Long-Horizon Robot Tasks vi (2026-09-21)

증류의 대상을 표현·능력에서 '판단 경계의 정렬'로 확장한다. 교사 모델의 결정 경계가 학생 태스크의 완료 기준과 자동으로 일치하지 않는다는 새 문제 설정을 추가한다.

→ [[sources/2026-09-21-stageguard-learning-stage-transitions-for-long-hor.md|상세 보기]]

### The Weight Is Over - Interactive Diffusion on Consumer GPUs (2026-09-22)

교사 텍스트 인코더의 출력 분포를 학생 소형 인코더+번역기에 전달하는 '조건화 계층 증류'라는 새 축을 추가한다. TIDE가 전체 모델 간 전이를 다뤘다면 본 논문은 모델-조건화기 경계의 번역 네트워크로 증류 단위를 세분화한다.

→ [[sources/2026-09-22-the-weight-is-over---interactive-diffusion-on-cons.md|상세 보기]]
