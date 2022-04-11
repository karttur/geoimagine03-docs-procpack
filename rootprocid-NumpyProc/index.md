---
layout: resume
title: NumpyProc
excerpt: Numpy data processing
rootprocid: NumpyProc
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'NumpyProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
