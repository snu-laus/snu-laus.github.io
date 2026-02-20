---
permalink: /publications
layout: page
title: "Publications"
---

## 2026
<br/>
{% for publi in site.data.publist2026 %}
<div class="pub">
  <img src="{{ site.url }}{{ site.baseurl }}/pubpic/{{ publi.image }}"/>
  <div class="text-content">
    <strong>{{ publi.authors }}&nbsp;&nbsp;<span class="pubyear">({{ publi.year }})</span></strong>
    <strong>{{ publi.title }}</strong>
    <em>{{ publi.display }}</em><br/>
    <strong style="border-bottom:1px dashed #277cea">{% if publi.link.url %}<a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer" style="display:inline;border-bottom:none">[link]</a>{% else %}[link]{% endif %}{% if publi.appendix %} <a href="{{ publi.appendix }}" style="display:inline;border-bottom:none">[appendix]</a>{% endif %}</strong>
  </div>
</div>
{% endfor %}

<br/><br/>

## 2025
<br/>
{% for publi in site.data.publist2025 %}
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

## 2024
<br/>
{% for publi in site.data.publist2024 %}
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

## 2023
<br/>
{% for publi in site.data.publist2023 %}
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
