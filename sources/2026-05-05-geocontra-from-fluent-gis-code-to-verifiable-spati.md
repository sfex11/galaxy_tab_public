# GeoContra: From Fluent GIS Code to Verifiable Spatial Analysis with Geography-Grounded Repair

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-05
**링크**: http://arxiv.org/abs/2605.00782v1

## 💡 핵심 인사이트

LLM 생성 코드의 '유창성'과 '도메인 의미론 준수' 사이에는 구조적 간극이 존재하며, 이를 도메인 특화 계약(geospatial contract)의 실행 가능한 형식화와 수리로 해소할 수 있다.

## 📖 분석

# GeoContra: 지리 정보 시스템 코드의 유창성과 검증 가능성 사이 간극

GeoContra는 LLM이 생성한 Python GIS 워크플로우가 지리적 의미론(좌표 체계, 위상, 단위, 공간적 타당성)을 보존하는지를 검증·수리하는 프레임워크로, 각 태스크를 '실행 가능한 지리 공간 계약(geospatial contract)'으로 형식화한다.

## 기존 Wiki와의 관계

[[algorithm-system-translation-gap]]의 구체적 현현이다: 지리적 의미론(CRS 메타데이터, 공간 술어, 위상 관계)이라는 '알고리즘 수준' 표현을 Python GIS 코드라는 '시스템 수준'으로 번역할 때 발생하는 의미론 상실을 계약 기반 수리(contract-grounded repair)로 해결한다. 기존에 이 간극이 에이전트 상태·체크포인트·희소 어텐션 도메인에서 논의되었다면, GeoContra는 지리 정보 과학이라는 도메인 특화적 실증을 제공한다.

[[execution-verification]]을 도메인 특화 계약으로 확장한다. 기존 Claw-Eval-Live가 에이전트 워크플로우의 실행 결과를 평가했다면, GeoContra는 '결과가 지리적으로 타당한가'라는 도메인 내재적 검증 기준을 실행 검증에 통합한다.

[[natural-language-to-formal-language]]의 지리 공간적 인스턴스다. 자연어 질문을 공간 술어·위상·CRS 메타데이터를 포함한 형식적 계약으로 번역하여, 기존 LTL 번역 연구가 다루던 '의미론적 번역의 어려움'을 공간 분석 도메인에서 구체화한다.

## 연결점

[[syntax-behavior-semantics-disentanglement]]: LLM이 생성한 GIS 코드가 '유창한 문법(syntax)'을 갖추면서도 '지리적 행동(behavior)'에서 위상 오류나 단위 혼동을 보이는 현상을 계약 수리로 교정한다는 점에서, 구문·행동·의미의 분리 문제를 지리 도메인에서 실증한다.

## 🔗 관련 논문

- diagnosing-cfg-interpretation-in-llms
- claw-eval-live-a-live-agent-benchmark-for-evolving
- syntax-is-easy-semantics-is-hard-evaluating-llms-f

## 🏷️ 엔티티

- [[entities/algorithm-system-translation-gap.md|algorithm-system-translation-gap]]
- [[entities/execution-verification.md|execution-verification]]
- [[entities/natural-language-to-formal-language.md|natural-language-to-formal-language]]
- [[entities/syntax-behavior-semantics-disentanglement.md|syntax-behavior-semantics-disentanglement]]
- [[entities/geospatial-contract.md|geospatial-contract]]

## 📐 개념

- [[concepts/coordinate-semantic-preservation.md|coordinate-semantic-preservation]]
- [[concepts/topology-aware-code-repair.md|topology-aware-code-repair]]
- [[concepts/geographic-plausibility-verification.md|geographic-plausibility-verification]]
- [[concepts/domain-grounded-contract-execution.md|domain-grounded-contract-execution]]

---
_LLM 분석으로 생성됨_
