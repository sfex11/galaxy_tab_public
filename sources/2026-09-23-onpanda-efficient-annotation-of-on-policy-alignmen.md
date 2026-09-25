# onPanda: Efficient Annotation of On-Policy Alignment Data for LLMs and Agents via Token-Level Correction

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-09-23  
**링크**: http://arxiv.org/abs/2609.24983v1

## 핵심 요약

We present onPanda, an interactive tool for efficiently annotating LLM alignment data and agent trajectories. onPanda adopts token-level correction as its core interaction: while reading a model response, the annotator locates the first inappropriate token and either picks a substitute from the model's candidate tokens or types the correct text via free-form editing. The system then truncates everything after that position and continues generation from the corrected prefix, repeating this locate...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

_없음_

## 추출된 개념

_없음_

## 메모

_자동 생성됨_

## 🔗 교차 참조

- → [[sources/2026-09-24-optimal-sequential-annotations-for-off-policy-eval]]: 저비용 모델(토큰 수준 교정, LLM judge) 출력에 고비용 인간 교정을 최적으로 배치해 주석 비용과 품질의 균형을 맞춘다는 효율적 주석 설계 문제를 공유한다.
- → [[sources/2026-09-23-who-does-what-in-ai-auditing-designing-human-ai-co]]: 정렬 데이터 주석과 감사라는 AI 산출물 품질 관리 작업에서 인간 판단과 AI 기여를 어떻게 분업할지 설계하는 인간-AI 협업 문제를 공유한다.
- → [[sources/2026-09-24-a2m-trace-optimized-agent-hijacking-in-the-mcp-eco]]: 에이전트 실행 궤적을 핵심 객체로 다룬다는 점에서 연결되며, onPanda의 궤적 주석·교정은 A2M 유형 하이재킹 궤적의 탐지·정제를 위한 방어 측 데이터 기반을 제공할 수 있다.
