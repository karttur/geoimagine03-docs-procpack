---
layout: rootprocess
title: SmapProc
excerpt: Manage SMAP processes
rootprocid: SmapProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'SmapProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
