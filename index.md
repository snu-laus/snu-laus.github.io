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

[서울대학교](https://www.snu.ac.kr/) [건축학과](https://architecture.snu.ac.kr/) 건축도시공간연구실(LAUS)은 1999년에 설립되어 🔴 공간분석, 🟢 건축계획, 🔵 도시설계 분야 연구를 수행하고 있습니다. 

The Lab for Architectural and Urban Space (LAUS), established in 1999 in the Department of Architecture and Architectural Engineering, Seoul National University, explores research topics of Urban and Architectural Space Analysis, Space Programming & Planning, and Urban Design Policy. 

---

대학원 진학 혹은 연구실에 관심이 있나요? [안내 페이지](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284)를 확인해주세요.
If you are interested in joining our lab as a graduate student, please check [this guide page](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284) first.

학부연구생을 모집합니다. [모집 공고 페이지](https://snu-laus.notion.site/2ab32921929280578f53ed18d64a12da?pvs=74)에 상세내용이 있습니다.

---

<br/>

## Newly Published

<div class="post-list">
{% assign all_pubs = site.data.publist_2026 | concat: site.data.publist_2025 %}
{% for area in all_pubs limit:3 %}
  {% include areacard1.html %}
{% endfor %}
</div>

---

<br/>

## News

<behold-widget feed-id="tSL96p4HaxD2zj1of56E"></behold-widget>
<script>
  (() => {
    const d=document,s=d.createElement("script");s.type="module";
    s.src="https://w.behold.so/widget.js";d.head.append(s);
  })();
</script>
