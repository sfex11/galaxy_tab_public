# Beyond Summaries: Structure-Aware Labeling of Code Changes with Large Language Models

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26100v1

## 💡 핵심 인사이트

이 논문이 핵심적으로 지적하는 것은, 코드 리뷰의 핵심은 텍스트가 아닌 **문서 구조**에 있다는 점이다. 기존 접근은 diff를 평면화하여 변경 의도를 상실하지만, 이 논문은 diff의 구조를 인식하여 변경의 성격(저위도 vs 고위도)와 유형(이동 vs 논리)을 분리하여 리뷰어의 정보 지형을 근본적으로 재설계한다.

## 📖 분석

# structure-aware-code-review

**카테고리**: 미분류
**생성일**: 2026-05-27

## 정의

기존 LLM 기반 코드 리뷰 접근이 코드 변경의 텍스트를 평면적으로 처리하는 근본적 한계를 지적한다. 코드 변경의 구조적 계층(파일→헝크→라인 변경)를 명시적으로 모델링하여, 변경 유형(이름 변경, 이동, 논리 수정 등)별로 리뷰 우선순위·필터링·자동화가 가능한 구조화된 라벨링 체계를 제안한다.

## 관련 논문

- sources/2605.26100-beyond-summaries-structure-aware-labeling-of-code-changes-with-large.md

### Beyond Summaries: Structure-Aware Labeling of Code Changes with Large La (2026-05-27)

이 논문은 기존 LLM 기반 코드 리뷰가 코드 변경의 텍스트를 평면적으로 처리하는 근본적 한계를 지적한다. 코드 변경의 구조적 계층(파일→헝크→라인 변경)를 명시적으로 모델링하여, 변경 유형(이름 변경, 이동, 논리 수정 등)별로 리뷰 우선순위·필터링·자동화가 가능한 구조화된 라벨링 체계를 제안한다.

## 🏷️ 엔티티

- [[entities/structure-aware-code-review.md|structure-aware-code-review]]
- [[entities/llm-as-code-reviewer.md|llm-as-code-reviewer]]
- [[entities/change-type-taxonomy.md|change-type-taxonomy]]

## 📐 개념

- [[concepts/diff-hierarchy.md|diff-hierarchy]]
- [[concepts/change-type-based-review-routing.md|change-type-based-review-routing]]

---
_LLM 분석으로 생성됨_
