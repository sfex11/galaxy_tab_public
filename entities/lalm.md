# Lalm

**카테고리**: AI/ML
**관련 논문**: 4편

## 정의

_Wiki 축적 중 (claude 분석 대기)_

## 논문에서 발견된 핵심 인사이트

- 다중 LALM의 독립적 추론 체인을 융합함으로써 오디오 질의응답의 추론 투명성과 검증 가능성을 동시에 확보할 수 있다.
- LLM은 텍스트 전용 사전학습만으로도 상당한 청각 도메인 지식을 습득하지만, 이 암묵적 지식과 실제 오디오 그라운딩 성능 사이에는 여전히 유의미한 갭이 존재하며, 백본 LLM의 선택이 LALM 성능을 좌우하는 핵심 요인이다.
- 텍스트 전용 사전학습만으로 LLM이 내재화한 청각 지식의 양이 LALM의 멀티모달 성능 상한선을 결정하며, AKB-2000 벤치마크를 통해 이를 체계적으로 정량화할 수 있다.
- LLM 백본이 텍스트 전용 사전학습만으로도 상당한 청각 지식을 인코딩하며, 이 사전 지식 수준이 LALM의 오디오 그라운딩 성능을 직접적으로 좌우한다.

## 전체 관련 논문 (4편)

- [[sources/2026-03-19-multi-source-evidence-fusion-for-audio-question-an.md|2026 03 19 multi source evidence fusion for audio question an.md]] (2026-03-19)
- [[sources/2026-03-21-how-auditory-knowledge-in-llm-backbones-shapes-aud.md|2026 03 21 how auditory knowledge in llm backbones shapes aud.md]] (2026-03-21)
- [[sources/2026-03-22-how-auditory-knowledge-in-llm-backbones-shapes-aud.md|2026 03 22 how auditory knowledge in llm backbones shapes aud.md]] (2026-03-22)
- [[sources/2026-03-23-how-auditory-knowledge-in-llm-backbones-shapes-aud.md|2026 03 23 how auditory knowledge in llm backbones shapes aud.md]] (2026-03-23)

### Evaluation of Automatic Speech Recognition Using Generative Large Lang (2026-04-25)

LLM 백본이 내재한 청각 지식이 LALM 성능 상한을 결정한다는 기존 발견을 평가 측면에서 보완한다—동일한 지식이 ASR 후보 평가의 신뢰성 상한선으로도 기능한다.

→ [[sources/2026-04-25-evaluation-of-automatic-speech-recognition-using-g.md|상세 보기]]
