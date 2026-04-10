# LoST: Level of Semantics Tokenization for 3D Shapes

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17995v1

## 💡 핵심 인사이트

3D 형상 토큰화에서 기하학적 세부 수준(LoD) 대신 의미론적 계층(Level of Semantics)을 사용하면 토큰 효율성과 생성 품질을 동시에 개선할 수 있다.

## 📖 분석

## LoST: Level of Semantics Tokenization for 3D Shapes

3D 형상의 생성 모델링에서 토큰화(tokenization)는 핵심적인 전처리 단계이다. 특히 최근 3D 생성에서 주목받는 자기회귀(autoregressive, AR) 모델에서 토큰화 방식은 생성 품질을 좌우한다. 기존 SOTA 방법들은 렌더링과 압축을 위해 설계된 기하학적 세부 수준(Level-of-Detail, LoD) 계층 구조에 의존하지만, 이는 토큰 효율성 측면에서 최적이 아니다.

LoST는 기하학적 계층 대신 **의미론적 수준(Level of Semantics)**에 기반한 토큰화를 제안한다. 3D 형상을 단순한 공간적 분할이 아닌, 의미적 구성 요소(부품, 기능적 단위 등)의 계층으로 분해하여 토큰 시퀀스를 구성한다. 이를 통해 토큰 수를 줄이면서도 형상의 의미적 구조를 보존할 수 있어, AR 모델의 생성 효율성과 품질을 동시에 향상시킨다.

이 연구는 토큰화 설계가 단순한 데이터 표현 문제가 아니라, 생성 모델이 학습하는 구조적 사전 지식(structural prior)을 결정한다는 점을 시사한다. 기존 NLP에서의 BPE, WordPiece 등 토큰화 전략이 언어 모델 성능에 미치는 영향과 유사한 맥락으로, 3D 도메인에서도 모달리티에 적합한 토큰화 전략의 중요성을 보여준다.

### 기존 Wiki와의 연결
- **Transformer** 엔티티와 관련: AR 기반 3D 생성 모델은 Transformer 아키텍처를 활용하며, 토큰화 방식이 Transformer의 시퀀스 처리 효율성에 직접적 영향을 미침
- 멀티모달 생성 및 표현 학습 연구들과 연결되며, 특히 시각적 표현의 구조화라는 관점에서 steerable visual representations 연구와 상보적 관계에 있음

## 🏷️ 엔티티

- [[entities/transformer.md|transformer]]

## 📐 개념

- [[concepts/tokenization.md|tokenization]]
- [[concepts/autoregressive-generation.md|autoregressive-generation]]
- [[concepts/3d-generation.md|3d-generation]]

---
_LLM 분석으로 재생성됨_
