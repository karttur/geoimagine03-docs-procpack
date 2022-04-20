---
layout: rootprocess
title: CopernicusProc
excerpt: Manage Copernicus processes
rootprocid: CopernicusProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'CopernicusProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
