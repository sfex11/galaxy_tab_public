# Mllm: 합성 분석

**생성일**: 2026-04-14  
**관련 논문**: 21편  
**최종 업데이트**: 2026-04-14

`wiki/entities/mllm.md`에 합성 분석 페이지를 작성했습니다. 21편의 논문을 4개 핵심 연구 축으로 정리했습니다:

1. **공간 추론과 3D 이해의 확장** — Loc3R-VLM, 3DCity-LLM, UniDriveVLA 등이 2D→3D→도시 규모로 확장
2. **에이전틱 MLLM과 메타인지** — MARCUS, Act Wisely, Stop Wandering 등이 자율적 행동과 자기 조절 능력에 수렴
3. **추론 효율화** — AdaptToken(토큰 축소) vs. VISOR(어텐션 희소화) vs. SpecEyes(파이프라인 병렬화)의 직교적 전략
4. **시각 표현과 학습 신뢰성** — Steerable Visual Representations의 새 패러다임과 RL 후훈련 환각 문제의 긴장 관계

특히 OpenVLThinkerV2(RL 후훈련으로 추론 개선) ↔ Hallucination in RL(환각 의존 단축학습 경고) 간의 긴장, Act Wisely ↔ Stop Wandering ↔ Chameleon의 메타인지 수렴이 주목할 만한 논문 간 관계입니다.