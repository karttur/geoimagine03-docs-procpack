---
layout: rootprocess
title: ModisPolar
excerpt: Processes for MODIS data in EASE2 north grid projecion
rootprocid: ModisPolar
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'ModisPolar' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
