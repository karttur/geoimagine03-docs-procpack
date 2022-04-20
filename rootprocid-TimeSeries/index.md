---
layout: rootprocess
title: TimeSeries
excerpt: Timeseries analysis
rootprocid: TimeSeries
search_omit: true
share: true
---

<ul class='post-list'>
{% for post in site.categories.subprocess %}
  {% if post.rootprocid == 'TimeSeries' %}
    {% include subprocess.html post=post %}
  {% endif %}
{% endfor %}
</ul>
