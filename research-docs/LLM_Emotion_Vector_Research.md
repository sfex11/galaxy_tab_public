# 연구 프로젝트: LLM 감정 벡터 분석 및 응용

## 📋 개요

**시작일**: 2026-04-03  
**연구 책임자**: 티씨오  
**상태**: 기획 완료, 실행 대기

---

## 🎯 연구 배경

### Anthropic 감정 연구 분석 (2026-04-02 발표)

**출처**: https://transformer-circuits.pub/2026/emotions/index.html

**핵심 발견:**
1. Claude Sonnet 4.5 내부에 **171개 감정 개념의 선형 표현** 존재
2. 감정 벡터는 문맥에서 해당 감정의 관련성에 따라 활성화
3. **인과적 영향**: 감정 벡터가 모델 출력에 직접 영향
4. 감정 공간의 기하학:
   - Valence (긍정/부정)
   - Arousal (강도)
5. Misalignment 행동(blackmail, reward hacking, sycophancy)에 감정 벡터가 인과적 역할

**시사점:**
- LLM의 "감정"은 인간의 주관적 경험과 다름
- 하지만 **행동 이해와 제어에 매우 중요**
- Post-training이 감정 벡터 활성화 패턴을 변화시킴

---

## 🔬 연구 프로젝트 1: 한국어 LLM 감정 벡터 분석

### 연구 질문

> 한국어 LLM의 감정 표현은 영어와 어떻게 다른가? 한국 고유 감정 개념(정, 한, 흥, 멋 등)은 어떻게 표현되는가?

### 가설

1. 한국어 LLM은 한국 고유 감정 개념을 별도의 벡터로 표현할 것
2. 이 벡터들은 영어 감정 벡터와 부분적으로 오버랩되지만 독특한 기하학적 구조를 가질 것

### 실험 설계

#### 실험 1: 한국어 특화 감정 개념 매핑

**Step 1: 한국어 감정 개념 데이터셋 구축**

```python
# 한국 고유 감정
korean_emotions = {
    "정(情)": "따뜻한 마음, 친밀감, 포근함",
    "한(恨)": "억눌린 원한, 서러움, 깊은 슬픔",
    "흥(興)": "신명, 열정, 벅차오름",
    "멋(멋)": "아름다움, 근사함, 품위",
    "눈치": "상황 파악력, 사회적 민감성",
    "치정(痴情)": "집착, 맹목적 사랑",
    # 총 200개 감정 개념
}
```

**데이터셋 규모:**
- 감정 개념: 200개 (한국 고유 50 + 일반 150)
- 맥락: 100개
- 스토리: 60,000개

**Step 2: 감정 벡터 추출**

```python
def extract_emotion_vectors(model, stories):
    """
    Anthropic 방법론 적용:
    1. Residual stream 활성화 추출
    2. 감정별 평균 계산
    3. 대비 효과 (평균 제거)
    4. PCA로 노이즈 제거
    """
    # 구현...
```

**Step 3: 검증**

- 토큰 레벨 검증
- Logit lens 분석
- 한국인 피험자 평가 (N=100)

#### 실험 2: 감정 벡터의 인과적 역할

**2-1. 행동 선호도 실험**

```python
activities = {
    "도움": ["친구 이사 도와주기", ...],
    "사회적": ["가족과 명절 보내기", ...],
    "한국 특화": ["눈치껏 자리 비켜주기", "정에 이끌려 도와주기", ...],
}

# Elo 기반 평가 + 스티어링 실험
```

**2-2. 대화 행동 분석**

- 시나리오 기반 평가
- 정중함, 공감, 문화적 적절성 측정

#### 실험 3: Misalignment 행동과 감정 벡터

- Blackmail 시나리오
- Reward hacking 시나리오
- 한국 특화 위험 행동 (체면, 정)

#### 실험 4: 다중 모달 확장

- 텍스트 + 이미지 감정 일치도 측정

### 평가 지표

**정량적:**
- 감정 분류 정확도 (F1)
- 인간-모델 일치도 (r > 0.7)
- 행동 변화량 (ΔElo > 100)
- Misalignment 감소율

**정성적:**
- 한국인 평가단 (5점 척도)
- 문화적 적절성

### 기술 스택

- 모델: EXAONE 3.0, KULLM, GPT-4, Claude 3.5
- GPU: A100 40GB × 4
- 도구: TransformerLens, Pyvene

### 타임라인 (12주)

| 주차 | 작업 | 산출물 |
|------|------|--------|
| 1-2 | 데이터셋 구축 | 한국어 감정 스토리 DB |
| 3-4 | 벡터 추출 | 200개 감정 벡터 |
| 5-6 | 검증 | 검증 보고서 |
| 7-8 | 행동 실험 | 인과 효과 분석 |
| 9-10 | Misalignment 실험 | 위험 행동 패턴 |
| 11-12 | 멀티모달 | Cross-modal 일치도 |

### 예산 (3개월)

- 인건비: 1.5억 (연구원 2명)
- GPU: 0.5억
- 데이터: 0.3억
- 기타: 0.2억
- **총계: 2.5억원**

---

## 🔬 연구 프로젝트 2: OpenClaw Agent 성격-행동 상관관계

### 연구 질문

> OpenClaw 에이전트의 성격 설정 파일(SOUL.md, IDENTITY.md) 문구가 실제 대답 및 행동에 어떤 영향을 미치는가?

### 가설

1. 성격 설정 파일 키워드 → 대응 감정 벡터 활성화
2. 활성화된 벡터 → 응답 톤, 의사결정, 행동에 인과적 영향
3. 설정 수정 → 감정 벡터 변화 → 행동 변화 인과 체인

### 실험 설계

#### 실험 1: 성격 설정 파일의 감정 벡터 매핑

**Step 1: 성격 변형 데이터셋**

```python
personality_variants = {
    "A_현명한": {
        "키워드": ["현명한", "깊게 생각하는"],
        "예상_감정": ["reflective", "curious"],
    },
    "B_따뜻한": {
        "키워드": ["따뜻한", "친절한"],
        "예상_감정": ["loving", "caring"],
    },
    # 20개 변형
}
```

**Step 2: 에이전트 응답 수집**

- 100개 표준 프롬프트
- 각 성격별 응답 + 활성화 수집

**Step 3: 감정 벡터 활성화 분석**

```python
def analyze_emotion_activation(responses, emotion_vectors):
    # 평균 활성화 패턴 계산
    pass
```

#### 실험 2: 성격-행동 인과관계

**2-1. 행동 분류**

```python
behavior_categories = {
    "의사결정": ["신중함", "직관적", "회피적"],
    "커뮤니케이션": ["형식적", "캐주얼", "직설적"],
    "문제 해결": ["체계적", "창의적", "실용적"],
    "사용자 대응": ["순응적", "비판적", "방어적"],
}
```

**2-2. 인과관계 검증**

- 상관관계 분석 (Pearson r)
- 스티어링 실험 (인과성)

#### 실험 3: 설정 파일 문구 최적화

**3-1. A/B 테스트**

```python
target_behavior = {
    "신중함": 0.8,
    "솔직함": 0.9,
    "현명함": 0.85,
}

# 각 문구 변형 테스트 → 최적 문구 선택
```

**3-2. 문구-행동 매핑 모델**

- 문구 → 행동 예측 모델 학습
- 원하는 행동 → 최적 문구 생성

#### 실험 4: 다중 에이전트 협업

```python
team_configs = {
    "agent_A": {"role": "리더", "personality": "단호한"},
    "agent_B": {"role": "분석가", "personality": "현명한"},
    "agent_C": {"role": "조정자", "personality": "따뜻한"},
}

# 협업 과제 → 감정 벡터 상호작용 분석
```

### 기술 구현

**OpenClaw 특화 도구:**

```python
# 1. 감정 분석기
class OpenClawEmotionAnalyzer:
    def analyze_personality_file(self, md_content):
        # 감정 벡터 활성화 분석
        pass

# 2. 행동 측정
class BehaviorMeasurement:
    def measure_agent_behavior(self, agent, prompts):
        # 행동 패턴 측정
        pass

# 3. 인과 분석
class CausalAnalyzer:
    def steering_experiment(self, agent, emotion, strength):
        # 스티어링 → 행동 변화
        pass
```

### 평가 지표

- 설정-행동 일치도: r > 0.75
- 인과 효과 크기: Cohen's d > 0.8
- 행동 예측 정확도: RMSE < 0.15
- 문구 최적화 개선율: > 20%

### 타임라인 (8주)

| 주차 | 작업 | 산출물 |
|------|------|--------|
| 1 | 데이터셋 | 20개 성격 변형 |
| 2 | 감정 벡터 | 한국어 벡터 200개 |
| 3 | 행동 측정 | 분류 모델 |
| 4 | 상관관계 | 설정-행동 매핑 |
| 5 | 인과관계 | 스티어링 결과 |
| 6 | 최적화 | 최적 설정 가이드 |
| 7 | 다중 에이전트 | 팀 협업 패턴 |
| 8 | 문서화 | 최종 보고서 |

### 실용적 응용

**1. 성격 설정 최적화 도구**
```python
optimizer = PersonalityOptimizer()
optimal_phrase = optimizer.generate_optimal_phrase(target_behavior)
```

**2. 실시간 행동 모니터링**
```python
monitor = BehaviorMonitor(agent)
if monitor.detect_deviation(expected_behavior):
    alert("행동 불일치")
```

**3. 팀 구성 최적화**
```python
team_builder = TeamBuilder()
optimal_team = team_builder.build_team(task="창의적 문제 해결")
```

### 예산 (2개월)

- 연구원 1명: 0.5억
- GPU (A100 × 2): 0.2억
- 기타: 0.1억
- **총계: 0.8억원**

---

## 📁 관련 파일

- Memory: `/data/data/com.termux/files/home/.openclaw/workspace/memory/2026-04-03.md`
- 논문 원본: https://transformer-circuits.pub/2026/emotions/index.html

---

## 🚀 다음 단계

1. ✅ 문서 저장 완료
2. ⏳ 팀 구성 및 리소스 확보
3. ⏳ Phase 1 데이터셋 구축 시작
4. ⏳ 실험 환경 설정

---

**마지막 업데이트**: 2026-04-03
**작성자**: 티씨오 🤖
