# Merging the Knowledge of LLMs for Automatic Speech Recognition

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-09-16
**링크**: http://arxiv.org/abs/2609.15743v1

## 💡 핵심 인사이트

외부 LM 지식을 디코딩 시점 런타임 주입에서 파라미터 병합으로 이전하면 LM 추론 비용 없이 언어 모델의 이득을 얻을 수 있으며, 지식 통합의 시점 선택 자체가 비용-품질 트레이드오프의 핵심 설계 변수다.

## 📖 분석

LM 퓨전(shallow fusion, density ratio)이 ASR 디코딩 중 외부 LM을 런타임 주입해 LM 추론 비용을 수반하는 방식이라면, 본 논문은 외부 LM 지식을 ASR 모델 파라미터에 사전 통합하는 **model-merging** 경로를 제시한다. 이는 [[runtime-to-parametric-memory-absorption]] 패턴의 정확한 실현 사례다 — 런타임 계층(퓨전 시 LM 추론)이 수행하던 지식 통합 기능이 파라미터 공간으로 '컴파일'되어 디코딩 시점 비용이 소멸한다.

[[parameter-decoupling]] 관점에서 LOCUS가 품질-비용을 별도 파라미터 축으로 분해했다면, 본 논문은 지식 통합의 시점(decoding-time → 사전 통합) 자체를 파라미터화 결정으로 전환한다. 외부 지식이 추론 시 매개될지 파라미터에 사전 흡수될지는 지식의 거주 위치 선택 문제가 되며, [[inference-time-behavior-control]]과 model-merging이 이 선택 공간의 양극을 형성한다.

[[knowledge-distillation]]과의 대비도 유의미하다 — 증류가 교사 출력 모방을 통한 지식 전이라면 병합은 가중치 공간에서의 직접 결합으로, 교사 추론 없이 텍스트 LM 지식이 음성 모델로 이전됨을 보여준다. [[audio-language-model]]·[[asr-evaluation]] 계열이 평가와 말단 생성에 집중했다면 본 논문은 텍스트 전용 LM 지식의 음성 도메인 흡수를 파라미터 수준 문제로 재정의하고, [[speech-llm]] 계열(RetroThinker, Nuha-Speech)의 종단간 통합과 별개의 하이브리드 경로를 추가한다.

## 🔗 관련 논문

- Evaluation of Automatic Speech Recognition Using Generative Large Language Model
- Unlocking Lossless Speedups in LLMs via Discrete Diffusion
- LOCUS: Task-Aware Low-Rank Post-Training for Token-Efficient Language Models
- RetroThinker: Enabling Retrospective Thinking in Speech LLMs
- Nuha-Speech: Building General-Purpose Arabic Speech-LLMs

## 🏷️ 엔티티

- [[entities/model-merging.md|model-merging]]
- [[entities/lm-fusion.md|lm-fusion]]
- [[entities/parameter-decoupling.md|parameter-decoupling]]
- [[entities/knowledge-distillation.md|knowledge-distillation]]
- [[entities/audio-language-model.md|audio-language-model]]
- [[entities/asr-evaluation.md|asr-evaluation]]
- [[entities/inference-time-behavior-control.md|inference-time-behavior-control]]

## 📐 개념

- [[concepts/runtime-to-parametric-memory-absorption.md|runtime-to-parametric-memory-absorption]]
- [[concepts/inference-time-behavior-control.md|inference-time-behavior-control]]
- [[concepts/parameter-decoupling.md|parameter-decoupling]]
- [[concepts/knowledge-integration-timing.md|knowledge-integration-timing]]

---
_LLM 분석으로 생성됨_
