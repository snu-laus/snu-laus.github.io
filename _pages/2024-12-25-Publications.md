---
permalink: /publications
layout: page
title: "Publications"
---

{% assign years = site.data.publist | map: "year" | uniq | sort: "desc" %}
{% for year in years %}
## {{ year }}
<br/>
{% assign pubs = site.data.publist | where: "year", year %}
{% for publi in pubs %}
<div class="pub">
  <img src="{{ site.url }}{{ site.baseurl }}/pubpic/{{ publi.image }}"/>
  <div class="text-content">
    <strong>{{ publi.authors }}&nbsp;&nbsp;<span class="pubyear">({{ publi.year }})</span></strong>
    <strong>{{ publi.title }}</strong>
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
{% endfor %}
