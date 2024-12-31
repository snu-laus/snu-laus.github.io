---
permalink: /publications
layout: page
title: "Publications"
---

## 2023
{% for publi in site.data.publist2023 %}
<div class="pub">
  <img src="{{ site.url }}{{ site.baseurl }}/pubpic/{{ publi.image }}"/>
  <strong>{{ publi.title }}</strong><br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.link.display }}<br/>
  {% if publi.link.url %}
  <strong><a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong><br/>
  {% else %}
  <br/>
  {% endif %}
</div>
{% endfor %}

<br/><br/>
