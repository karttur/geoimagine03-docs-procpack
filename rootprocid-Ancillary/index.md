---
layout: resume
title: Ancillary
excerpt: Ancillary data processing
rootprocid: Ancillary
search_omit: true
share: true
---

<h1 class='foot-description'>Sub processes</h1>
<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Ancillary' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
