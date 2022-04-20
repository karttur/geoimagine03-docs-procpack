---
layout: rootprocess
title: ManageProject
excerpt: Manage projects
rootprocid: ManageProject
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'ManageProject' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
