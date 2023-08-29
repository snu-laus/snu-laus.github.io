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

<!---

<table style="border-collapse: collapse; width: 100%; border:none;" border="1" align="left">
<tbody>
<tr><td style=" border-left-width: 0px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; padding-left: 0px; padding-top: 0px; padding-bottom: 0px; padding-right: 0px;"><span style=" font-family: 'Poppins', sans-serif; font-size: 400%">LAUS</span></td></tr>
<tr><td style="border-left-width: 0px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; padding-left: 0px; padding-top: 0px; padding-bottom: 0px; padding-right: 0px;"><span style=" font-family: 'Poppins', sans-serif; font-size: 150%">Lab for Architecture and Urban Space</span></td></tr>
</tbody>
</table>

<br/>

-->

# Lab for Architectural and Urban Space

서울대학교 건축학과 건축도시공간연구실(LAUS)은 1999년에 설립되어 공간분석, 건축계획, 도시설계 및 분석 분야 연구를 수행하고 있습니다. 

The Lab for Architectural and Urban Space (LAUS), established in 1999 in the Department of Architecture and Architectural Engineering, Seoul National University, explores research topics of Spatial Analysis, Architectural Planning, and Urban Design and Analytics. 

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

<figure data-behold-id="tSL96p4HaxD2zj1of56E"></figure>
<script src="https://w.behold.so/widget.js" type="module"></script>
