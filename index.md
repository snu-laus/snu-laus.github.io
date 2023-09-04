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

# Lab for Architectural and Urban Space

서울대학교 건축학과 건축도시공간연구실(LAUS)은 1999년에 설립되어 <mark >**공간분석, 건축계획, 도시설계**</mark> 분야 연구를 수행하고 있습니다. 

The Lab for Architectural and Urban Space (LAUS), established in 1999 in the Department of Architecture and Architectural Engineering, Seoul National University, explores research topics of Urban and Architectural Space Analysis, Space Programming & Planning, and Urban Design Policy. 

<br/>

<div class="container">
    <div class="post-list" itemscope="" itemtype="http://schema.org/Blog">
    {% for area in site.areas %}
    {% include areacard.html %}
    {% endfor %}
    </div>
</div>


<br/>

<figure data-behold-id="tSL96p4HaxD2zj1of56E"></figure>
<script src="https://w.behold.so/widget.js" type="module"></script>
