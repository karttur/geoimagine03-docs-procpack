---
layout: rootprocess
title: DemProc
excerpt: DEM data processing
rootprocid: DemProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'DemProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
