---
permalink: /publications
layout: page
title: "Publications"
---

## 2023
{% for publi in site.data.publist2023 %}
<div class="pub">
  <img src="{{ site.url }}{{ site.baseurl }}/pubpic/{{ publi.image }}"/>
  <div class="text-content">
    <div class="text-item">{{ publi.authors }}&nbsp;&nbsp;<span class="pubyear">({{ publi.year }})</span></div>
    <div class="text-item">{{ publi.title }}</div>
    <em>{{ publi.display }}</em><br/>
    {% if publi.link.url %}
    <strong><a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong>
    {% else %}
    &nbsp;
    {% endif %}
  </div>
</div>
{% endfor %}

<br/><br/>
