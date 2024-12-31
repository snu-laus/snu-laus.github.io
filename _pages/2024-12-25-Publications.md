---
permalink: /publications
layout: page
title: "Publications"
---

{% for publi in site.paper.publist2022 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 20px 20px 20px"> 
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
