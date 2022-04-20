---
layout: rootprocess
title: projsys
excerpt: Projection system data import
rootprocid: projsys
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'projsys' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
