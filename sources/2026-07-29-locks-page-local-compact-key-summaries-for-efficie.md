# LOCKS: Page-Local Compact Key Summaries for Efficient Long-Context Decoding

**타입**: 논문  
**출처**: arXiv  
**날짜**: 2026-07-29  
**링크**: http://arxiv.org/abs/2607.24555v1

## 핵심 요약

Serving large language models at long context is bottlenecked by the key-value (KV) cache, which is read in full at every decode step. Attention keys are locally low-rank though globally high-rank: shared low-rank bases discard page-specific directions that a page's own compact basis retains. LOCKS gives every page its own spectral summary (resident, about a tenth the cache's size), reconstructs within-page logits, estimates each page's attention mass by log-sum-exp, and attends only the top pag...

## 인사이트

1. 추출 필요
2. 추출 필요
3. 추출 필요

## 응용 가능성

1. 추출 필요
2. 추출 필요

## 추출된 엔티티

- [[Transformer]]

## 추출된 개념

_없음_

## 메모

_자동 생성됨_
