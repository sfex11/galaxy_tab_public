---
layout: default
title: "엔티티"
---

# 🏷️ 엔티티

연구 대상이 되는 구체적 객체들

{% assign entities = site.entities %}

**총 {{ entities.size }}개의 엔티티**

---

{% for entity in entities %}

## [{{ entity.title }}]({{ entity.url | relative_url }})

{{ entity.content | strip_html | truncatewords: 50 }}

---

{% endfor %}
