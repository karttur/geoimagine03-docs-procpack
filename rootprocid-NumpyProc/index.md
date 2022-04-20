---
layout: rootprocess
title: NumpyProc
excerpt: Numpy data processing
rootprocid: NumpyProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'NumpyProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
