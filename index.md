---
#
# You don't need to edit this file, it's empty on purpose.
# Edit sleeks's default layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
title: 건축도시공간연구실
secondtitle: Lab for Architectural & Urban Space
---

<br/><br/>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap" rel="stylesheet">
<span style=" font-family: 'Poppins', sans-serif;">LAUS</span>

<h2>Lab for Architecture and Urban Space</h2>
<br/>
건축도시공간연구실(LAUS)은 공간을 해석하고, 기획·계획하는 대학원 연구실입니다. 건축 및 도시공간의 사회적·문화적 배경을 이해하고, 논리적인 방법론을 통해 건조환경 계획을 발전시키고자 합니다.

<br/><br/>

## Research
<div class="container">
    <div class="post-list" itemscope="" itemtype="http://schema.org/Blog">
    {% assign sortedNews1 = site.areas | sort: 'date' | reverse %}
    {% assign areas1 = sortedNews1 | slice: 0, 3 %}
    {% for area in areas1 %}
    {% include areacard.html %}
    {% endfor %}
    <!-- {% include pagination.html %} -->
    </div>
</div>

<style>
    table th {
        font-size:1.1rem;
        font-weight:bold;
        border: 0px;
        padding : 0px;
        width: 10%;
        background-color : #ffffff;
    }
    thead {
        border: 0px;
    }
    .summary {
      font-size: 1rem;
      font-weight: normal;
    }
</style>


## News
<div class="container">
    <div class="post-list" itemscope="" itemtype="http://schema.org/Blog">
    {% assign sortedNews2 = site.news | sort: 'date' | reverse %}
    {% assign areas2 = sortedNews2 | slice: 0, 3 %}
    {% for area in areas2 %}
    {% include areacard.html %}
    {% endfor %}
    <!-- {% include pagination.html %} -->
    </div>
</div>

<style>
    table th {
        font-size:1.1rem;
        font-weight:bold;
        border: 0px;
        padding : 0px;
        width: 10%;
        background-color : #ffffff;
    }
    thead {
        border: 0px;
    }
    .summary {
      font-size: 1rem;
      font-weight: normal;
    }
</style>


