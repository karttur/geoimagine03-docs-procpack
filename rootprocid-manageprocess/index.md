---
layout: rootprocess
title: manageprocess
excerpt: Manage database defined process
rootprocid: manageprocess
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'manageprocess' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
