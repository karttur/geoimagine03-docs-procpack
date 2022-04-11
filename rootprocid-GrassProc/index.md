---
layout: resume
title: GrassProc
excerpt: Grass GIS processes binding
rootprocid: GrassProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'GrassProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
