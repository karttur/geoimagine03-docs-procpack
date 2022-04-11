---
layout: resume
title: projsys
excerpt: Projection system data import
rootprocid: projsys
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'projsys' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
