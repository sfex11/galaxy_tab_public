---
layout: default
title: "개념"
---

# 💡 개념

연구에서 사용되는 추상적 개념이나 방법론

{% assign concepts = site.concepts %}

**총 {{ concepts.size }}개의 개념**

---

{% for concept in concepts %}

## [{{ concept.title }}]({{ concept.url | relative_url }})

{{ concept.content | strip_html | truncatewords: 50 }}

---

{% endfor %}
