---
layout: default
title: "OpenClaw Wiki"
---

# 🏠 OpenClaw Wiki

**Karpathy 패턴 기반 LLM Wiki 시스템**

![Wiki Architecture](https://img.shields.io/badge/Status-Active-brightgreen)
![Papers](https://img.shields.io/badge/Papers-63-blue)
![Last Update](https://img.shields.io/badge/Updated-2026--04--05-orange)

---

## 📊 Wiki 통계

| 카테고리 | 수량 |
|----------|------|
| 📄 Sources (논문) | 63개 |
| 🏷️ Entities | 1개 |
| 💡 Concepts | 1개 |
| **Total** | **68개** |

---

## 🎯 최근 활동

### 2026-04-05
- ✅ Karpathy LLM Wiki 패턴 구현 완료
- ✅ 63개 일일 요약 마이그레이션
- ✅ GitHub 연동 (자동 동기화)
- ✅ Cross-reference 자동 생성

### 2026-04-03
- 📚 Anthropic 감정 벡터 연구 분석
- 🔬 연구 프로젝트 2개 기획
- 🛠️ 10대 신기술 조사

---

## 🔗 바로가기

### 📚 연구 자료
- [**Sources (논문 요약)**]({{ "/sources" | relative_url }}) - 63편의 논문 요약
- [**Entities**]({{ "/entities" | relative_url }}) - 연구 대상 엔티티
- [**Concepts**]({{ "/concepts" | relative_url }}) - 연구 개념 및 방법론

### 🔬 연구 프로젝트
- [**LLM 감정 벡터 연구**]({{ "/research/emotion-vector" | relative_url }})
- [**신기술 조사**]({{ "/research/technologies" | relative_url }})

### 📖 문서
- [Wiki Schema]({{ "/WIKI_SCHEMA" | relative_url }}) - Wiki 운영 규칙
- [Index]({{ "/index" | relative_url }}) - 전체 카탈로그
- [Log]({{ "/log" | relative_url }}) - 작업 타임라인

---

## 🤖 시스템 정보

**Wiki 엔진**: Karpathy LLM Wiki Pattern  
**자동화**: OpenClaw + Cron Jobs (8개)  
**저장소**: [GitHub](https://github.com/sfex11/galaxy_tab_public)  
**관리자**: 티씨오 🤖

---

## 📈 자동화 파이프라인

```
논문 수집 (9시, 10시)
    ↓
일일 요약 생성 (매시간)
    ↓
Wiki 통합 (18:30)
    ↓
Lint 체크 (일요일 19시)
    ↓
Cross-reference (일요일 1시간마다)
    ↓
Git 커밋 & GitHub 푸시 (매일 20시)
```

---

> 💡 **팁**: 이 Wiki는 [Karpathy의 LLM Wiki 패턴](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)을 기반으로 구축되었습니다.
