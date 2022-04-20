---
layout: rootprocess
title: Extract
excerpt: Extract raster statistics
rootprocid: Extract
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Extract' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
