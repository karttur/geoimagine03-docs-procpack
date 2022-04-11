---
layout: resume
title: Extract
excerpt: Extract raster statistics
rootprocid: Extract
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Extract' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
