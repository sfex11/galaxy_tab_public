# Emotion Vector

**분야**: Representation, Control  
**생성일**: 2026-04-05  
**최종 수정**: 2026-04-05

## 정의

LLM 내부에서 감정 개념을 표현하는 선형 벡터 표현. Claude Sonnet 4.5에서 171개 감정 개념이 발견됨.

## 작동 원리

### 1. 추출
```python
# 감정 스토리 데이터셋으로 학습
stories = generate_emotional_stories(emotion="happy")
activations = model.get_residual_stream(stories)
emotion_vector = activations.mean() - global_mean
```

### 2. 프로빙
```python
# 새 입력에서 감정 활성화 측정
activation = model.get_activation(input)
emotion_score = activation @ emotion_vector
```

### 3. 스티어링
```python
# 행동 제어
steered_activation = activation + 0.5 * emotion_vector
output = model.generate(steered_activation)
```

## 핵심 발견 (Anthropic 2026)

1. **171개 감정 벡터** 존재
2. **인과적 영향**: 감정 벡터가 행동을 직접 제어
3. **기하학적 구조**: Valence (긍정/부정) + Arousal (강도)
4. **Misalignment 연관**: desperation, lack_of_calm이 위험 행동 유발

## 한국 특화 감정

한국 고유 감정 개념:
- **정(情)**: 따뜻함, 친밀감
- **한(恨)**: 억눌린 원한
- **흥(興)**: 신명, 열정
- **눈치**: 사회적 민감성

## 장점

- 미세조정 없이 행동 제어
- 실시간 조정 가능
- 인과관계 명확

## 한계

- 단순한 행동만 제어 가능
- 복잡한 성격 특성은 어려움
- 부작용 가능성

## 관련 엔티티

- [[entities/llm-agent]] - 감정 벡터가 적용되는 주체
- [[entities/claude-3.5]] - 감정 벡터가 발견된 모델

## 관련 소스

- [[sources/2026-04-02-Emotion-Research]] - Anthropic 감정 연구 (예정)

## 관련 개념

- [[concepts/activation-steering]] - 활성화 조향
- [[concepts/representation-engineering]] - 표현 엔지니어링
- [[concepts/probing-classifier]] - 프로빙 분류기

## 응용 분야

1. **AI 안전성**: 위험 행동 조기 감지 및 차단
2. **성격 설정**: 에이전트 성격 실시간 조정
3. **사용자 경험**: 감정 인식 및 적응적 응답

## 외부 참조

- [Anthropic Emotion Research](https://transformer-circuits.pub/2026/emotions/)
- [Representation Engineering Paper](https://arxiv.org/)

## 메모

연구 프로젝트 1에서 한국어 특화 감정 벡터 분석 예정.
