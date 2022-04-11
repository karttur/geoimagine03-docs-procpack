---
layout: resume
title: SentinelProcess
excerpt: Manage Sentinel processes
rootprocid: SentinelProcess
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'SentinelProcess' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
