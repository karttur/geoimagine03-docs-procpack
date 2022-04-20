---
layout: rootprocess
title: Export
excerpt: Export spatial data
rootprocid: Export
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Export' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
