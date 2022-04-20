---
layout: rootprocess
title: GrassDemProc
excerpt: Grass data processing
rootprocid: GrassDemProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'GrassDemProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
