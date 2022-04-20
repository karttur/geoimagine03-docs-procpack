---
layout: rootprocess
title: ManageRegion
excerpt: Create tiles from regional data
rootprocid: ManageRegion
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'ManageRegion' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
