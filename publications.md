---
layout: default
title: 研究実績
---

このページでは、研究室の所属学生の研究成果を紹介しています。教員の個人発表については、[researchmap]({{ site.researchmap }})をご覧ください。

{% for y in site.data.publications %}
## {{ y.year }}年

<ol class="pub-list">
{% for p in y.items %}
  <li>{{ p.authors }}「<span class="pub-title">{{ p.title }}</span>」{{ p.venue }}{% if p.place %}、{{ p.place }}{% endif %}{% if p.date %}、{{ p.date }}{% endif %}</li>
{% endfor %}
</ol>
{% endfor %}
