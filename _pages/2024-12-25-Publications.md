---
permalink: /publications
layout: page
title: "Publications"
---

## 2026
<br/>
{% for publi in site.data.publist_2026 %}
<div class="pub">
  <img src="/assets/pubpic/{{ publi.image }}"/>
  <div class="text-content">
    <strong>{{ publi.authors }}&nbsp;&nbsp;<span class="pubyear">({{ publi.year }})</span></strong>
    <strong>{{ publi.title }}</strong>
    <em>{{ publi.display }}</em><br/>
    <div class="pub-links">{% if publi.link.url %}<strong><a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong>{% else %}<strong>[link]</strong>{% endif %}{% if publi.link.appendix %} <strong><a href="{{ publi.link.appendix }}">[appendix]</a></strong>{% endif %}{% if publi.link.map %} <strong><a href="{{ publi.link.map }}" target="_blank" rel="noopener noreferrer">[map]</a></strong>{% endif %}</div>
  </div>
</div>
{% endfor %}

<br/><br/>

## 2025
<br/>
{% for publi in site.data.publist_2025 %}
<div class="pub">
  <img src="/assets/pubpic/{{ publi.image }}"/>
  <div class="text-content">
    <strong>{{ publi.authors }}&nbsp;&nbsp;<span class="pubyear">({{ publi.year }})</span></strong>
    <strong>{{ publi.title }}</strong>
    <em>{{ publi.display }}</em><br/>
    <div class="pub-links">{% if publi.link.url %}<strong><a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong>{% else %}&nbsp;{% endif %}{% if publi.link.map %} <strong><a href="{{ publi.link.map }}" target="_blank" rel="noopener noreferrer">[map]</a></strong>{% endif %}</div>
  </div>
</div>
{% endfor %}

<br/><br/>

## 2024
<br/>
{% for publi in site.data.publist_2024 %}
<div class="pub">
  <img src="/assets/pubpic/{{ publi.image }}"/>
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
{% for publi in site.data.publist_2023 %}
<div class="pub">
  <img src="/assets/pubpic/{{ publi.image }}"/>
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
