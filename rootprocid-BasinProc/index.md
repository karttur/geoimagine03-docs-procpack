---
layout: resume
title: BasinProc
excerpt: basin processes
rootprocid: BasinProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'BasinProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
