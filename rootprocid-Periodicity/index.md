---
layout: resume
title: Periodicity
excerpt: Period settings
rootprocid: Periodicity
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Periodicity' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
