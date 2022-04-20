---
layout: rootprocess
title: DatabaseProc
excerpt: Database processing
rootprocid: DatabaseProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'DatabaseProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
