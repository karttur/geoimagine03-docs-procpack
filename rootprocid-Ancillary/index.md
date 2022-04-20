---
layout: rootprocess
title: Ancillary
excerpt: Ancillary data processing
rootprocid: Ancillary
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'Ancillary' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
