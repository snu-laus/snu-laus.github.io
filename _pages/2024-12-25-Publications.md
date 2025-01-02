---
permalink: /publications
layout: page
title: "Publications"
---

---
permalink: /publications
layout: page
title: "Publications"
---

{% for year in [2024, 2023] %}
## {{ year }}
<br/>
{% for publi in site.data['publist' | append: year] %}
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
