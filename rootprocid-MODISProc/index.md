---
layout: resume
title: MODISProc
excerpt: Manage MODIS processes
rootprocid: MODISProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'MODISProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
