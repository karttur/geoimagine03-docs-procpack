---
layout: resume
title: CopernicusProc
excerpt: Manage Copernicus processes
rootprocid: CopernicusProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'CopernicusProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
