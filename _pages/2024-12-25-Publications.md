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
    {{ publi.authors }} <span class="pubyear">({{ publi.year }})</span>
    <strong>{{ publi.title }}</strong>
    <em>{{ publi.display }}</em><br/>
    {% if publi.link.url %}
    <strong><a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong><br/>
    {% else %}
    <br/>
    {% endif %}
  </div>
</div>
{% endfor %}

<br/><br/>
