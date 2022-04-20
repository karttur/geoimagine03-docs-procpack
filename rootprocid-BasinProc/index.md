---
layout: rootprocess
title: BasinProc
excerpt: basin processes
rootprocid: BasinProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'BasinProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
