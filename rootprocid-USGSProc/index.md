---
layout: resume
title: USGSProc
excerpt: Manage USGS processes
rootprocid: USGSProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'USGSProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
