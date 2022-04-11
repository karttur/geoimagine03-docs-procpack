---
layout: resume
title: SmapProc
excerpt: Manage SMAP processes
rootprocid: SmapProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'SmapProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
