# How Auditory Knowledge in LLM Backbones Shapes Audio Language Models: A Holistic Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-23
**링크**: http://arxiv.org/abs/2603.19195v1

## 💡 핵심 인사이트

LLM 백본이 텍스트 전용 사전학습만으로도 상당한 청각 지식을 인코딩하며, 이 사전 지식 수준이 LALM의 오디오 그라운딩 성능을 직접적으로 좌우한다.

## 📖 분석

## How Auditory Knowledge in LLM Backbones Shapes Audio Language Models: A Holistic Evaluation

본 논문은 Large Audio Language Models(LALMs)의 백본으로 사용되는 LLM이 텍스트 전용 사전학습을 통해 얼마나 많은 청각 지식(auditory knowledge)을 인코딩하는지, 그리고 이것이 하류 성능에 어떤 영향을 미치는지를 체계적으로 분석한다.

### 핵심 방법론
세 가지 평가 설정을 통해 LLM의 청각 지식을 비교한다: (1) AKB-2000이라는 큐레이션된 벤치마크를 활용한 직접 프로빙(direct probing), (2) LLM이 텍스트 기반으로 추론하는 캐스케이드 평가(cascade evaluation), (3) 오디오가 직접 입력되는 오디오-그라운딩 설정. 이를 통해 텍스트 전용 학습에서 획득한 청각 지식의 폭과 깊이를 정량화한다.

### 주요 발견
- LLM 백본의 텍스트 기반 청각 지식 수준이 LALM의 최종 성능과 유의미한 상관관계를 가짐
- 모델 크기와 사전학습 데이터의 다양성이 청각 지식 인코딩에 핵심적 역할
- 오디오 인코더와 LLM 백본 간의 지식 보완 관계가 존재하며, 백본의 사전 지식이 풍부할수록 오디오 그라운딩 효율이 높아짐

### 기존 연구와의 연결
본 연구는 [[entities/lalm.md|lalm]] 엔티티와 직접적으로 관련되며, 기존 Multi-Source Evidence Fusion for Audio Question Answering 연구가 다룬 [[concepts/audio-question-answering.md|audio question answering]], [[concepts/evidence-fusion.md|evidence fusion]], [[concepts/reasoning-chain.md|reasoning chain]] 개념을 확장한다. 특히 오디오 QA 태스크에서 LLM 백본의 역할을 재조명한다는 점에서 상호보완적이다. 또한 [[concepts/audio-language-model.md|audio language model]] 개념과 밀접하게 연결되며, LLM의 멀티모달 확장 맥락에서 [[concepts/multimodal-learning.md|multimodal learning]]과도 관련된다.

## 🔗 관련 논문

- Multi-Source Evidence Fusion for Audio Question Answering

## 🏷️ 엔티티

- [[entities/lalm.md|LALM]]

## 📐 개념

- [[concepts/audio-language-model.md|audio-language-model]]
- [[concepts/audio-question-answering.md|audio-question-answering]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/evidence-fusion.md|evidence-fusion]]
- [[concepts/multimodal-learning.md|multimodal-learning]]

---
_LLM 분석으로 재생성됨_
