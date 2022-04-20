---
layout: rootprocess
title: LayoutProc
excerpt: Manage Layout processes
rootprocid: LayoutProc
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'LayoutProc' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
