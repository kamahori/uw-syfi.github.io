---
layout: page
title: "News"
---

{% for item in site.data.news.news limit:5 %}
<div class="row g-5 mb-5">
  <div class="col-md-12">
    <span class="badge bg-secondary">{{ item.date }}</span>
    <a href="{{ site.github.url }}{{ item.link }}">{{ item.title }}</a>
  </div>
</div>
{% endfor %}
