# How Auditory Knowledge in LLM Backbones Shapes Audio Language Models: A Holistic Evaluation

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-21
**링크**: http://arxiv.org/abs/2603.19195v1

## 💡 핵심 인사이트

LLM은 텍스트 전용 사전학습만으로도 상당한 청각 도메인 지식을 습득하지만, 이 암묵적 지식과 실제 오디오 그라운딩 성능 사이에는 여전히 유의미한 갭이 존재하며, 백본 LLM의 선택이 LALM 성능을 좌우하는 핵심 요인이다.

## 📖 분석

## How Auditory Knowledge in LLM Backbones Shapes Audio Language Models: A Holistic Evaluation

본 논문은 Large Audio Language Models(LALMs)의 백본으로 사용되는 LLM이 텍스트 전용 사전학습만으로 얼마나 많은 청각적 지식(auditory knowledge)을 인코딩하는지, 그리고 이것이 다운스트림 성능에 어떤 영향을 미치는지를 체계적으로 분석한다.

### 핵심 방법론
세 가지 평가 설정을 통해 LLM 백본의 청각 지식을 비교한다: (1) **AKB-2000 직접 프로빙** — 청각 지식의 폭과 깊이를 측정하는 큐레이션된 벤치마크, (2) **캐스케이드 평가** — LLM이 오디오 캡션 등 텍스트 중간 표현을 통해 추론하는 설정, (3) **오디오 그라운딩 평가** — 실제 오디오 입력과 결합된 LALM 성능 측정.

### 주요 발견
- 텍스트 전용 사전학습만으로도 LLM은 상당한 수준의 청각 도메인 지식을 습득함
- 그러나 이 텍스트 기반 청각 지식과 실제 오디오 그라운딩 성능 사이에는 갭이 존재
- LLM 백본의 선택이 LALM의 최종 성능에 유의미한 영향을 미침

### 기존 Wiki와의 연결
본 논문은 기존 Wiki의 [[entities/lalm.md|lalm]] 엔티티와 직접적으로 관련되며, 특히 Multi-Source Evidence Fusion for Audio Question Answering 논문이 다룬 오디오 질의응답 및 증거 융합 패러다임의 연장선에 있다. 또한 reasoning-chain 개념과도 연결되는데, LLM 백본이 캐스케이드 방식으로 청각 정보를 추론하는 과정이 이에 해당한다. evidence-fusion 개념과도 관련이 있으며, 텍스트 기반 지식과 오디오 모달리티를 결합하는 방식이 멀티소스 증거 융합의 한 형태로 볼 수 있다.

## 🔗 관련 논문

- Multi-Source Evidence Fusion for Audio Question Answering

## 🏷️ 엔티티

- [[entities/lalm.md|LALM]]

## 📐 개념

- [[concepts/audio-question-answering.md|audio-question-answering]]
- [[concepts/reasoning-chain.md|reasoning-chain]]
- [[concepts/evidence-fusion.md|evidence-fusion]]
- [[concepts/audio-language-model.md|audio-language-model]]
- [[concepts/multimodal-learning.md|multimodal-learning]]

---
_LLM 분석으로 재생성됨_
