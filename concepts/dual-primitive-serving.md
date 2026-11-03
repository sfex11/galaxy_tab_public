# 이원 원시 연산 서빙

**생성일**: 2026-11-03

## 정의

System One(범주적 결정) 워크로드에는 상태 분기(exact state forking)를, System Two(자기회귀 추론)에는 토큰 생성을 원시 연산으로 동시에 노출하는 서빙 추상화. 서빙의 기본 단위를 토큰 생성에서 상태 분기로 이동시키되, 전면 대체가 아닌 두 원시 연산의 공존을 요구한다.

## 관련 논문

- agent-native-serving
- decoder-primitive-redefinition
- decision-model-serving
- exact-state-forking
- autoregressive-generation
- dual-process-agent

---
_자동 Wiki Query에서 추출됨_
