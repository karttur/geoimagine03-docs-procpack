---
layout: rootprocess
title: GrassProc
excerpt: Grass GIS processes binding
rootprocid: GrassProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'GrassProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
