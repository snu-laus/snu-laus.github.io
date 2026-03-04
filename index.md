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

## Publications

<div class="container">
  {% comment %}
    1️⃣ _data 안의 모든 publist* 파일 자동 합치기
  {% endcomment %}
  {% assign all_pubs = "" | split: "" %} <!-- 빈 배열 초기화 -->

  {% for key in site.data %}
    {% if key contains "publist" %}
      {% assign all_pubs = all_pubs | concat: site.data[key] %}
    {% endif %}
  {% endfor %}

  {% comment %}
    2️⃣ 연도 기준 내림차순 정렬
  {% endcomment %}
  {% assign sorted_pubs = all_pubs | sort: "year" | reverse %}

  {% comment %}
    3️⃣ 상위 3개 선택
  {% endcomment %}
  {% assign latest3_pubs = sorted_pubs | slice: 0,3 %}

  {% comment %}
    4️⃣ 반복문으로 썸네일 + 모달 생성
  {% endcomment %}
  {% for pub in latest3_pubs %}
    <!-- 썸네일 -->
    <div class="pub-thumb" style="display:inline-block; margin:10px;">
      <img src="/assets/pubpic/{{ pub.image }}" alt="{{ pub.title }}" style="width:200px; cursor:pointer;" id="thumb{{ forloop.index }}">
    </div>

    <!-- 모달 -->
    <div id="modal{{ forloop.index }}" class="modal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.8); z-index:1000;">
      <div class="modal-content" style="background:white; max-width:600px; margin:5% auto; padding:20px; border-radius:10px; position:relative;">
        <span class="closeModal" data-modal="modal{{ forloop.index }}" style="position:absolute; top:10px; right:15px; font-size:28px; cursor:pointer;">&times;</span>

        <!-- 모달 안 내용 -->
        <img src="/assets/pubpic/{{ pub.image }}" style="width:100%; margin-bottom:15px;">
        <strong>{{ pub.authors }}&nbsp;&nbsp;<span class="pubyear">({{ pub.year }})</span></strong><br/>
        <strong>{{ pub.title }}</strong><br/>
        <em>{{ pub.display }}</em><br/>
        {% if pub.description %}<p>{{ pub.description }}</p>{% endif %}
        <div class="pub-links">
          {% if pub.link.url %}
            <strong><a href="{{ pub.link.url }}" target="_blank" rel="noopener noreferrer">[link]</a></strong>
          {% else %}
            &nbsp;
          {% endif %}
          {% if pub.appendix %}
            <strong><a href="{{ pub.appendix }}">[appendix]</a></strong>
          {% endif %}
          {% if pub.map %}
            <strong><a href="{{ pub.map }}" target="_blank" rel="noopener noreferrer">[map]</a></strong>
          {% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>

{% comment %}
  5️⃣ 모달 JS
{% endcomment %}
<script>
  {% for pub in latest3_pubs %}
    const modal{{ forloop.index }} = document.getElementById("modal{{ forloop.index }}");
    const thumb{{ forloop.index }} = document.getElementById("thumb{{ forloop.index }}");
    const close{{ forloop.index }} = modal{{ forloop.index }}.querySelector(".closeModal");

    thumb{{ forloop.index }}.onclick = function() {
      modal{{ forloop.index }}.style.display = "block";
    }

    close{{ forloop.index }}.onclick = function() {
      modal{{ forloop.index }}.style.display = "none";
    }

    window.onclick = function(event) {
      if (event.target == modal{{ forloop.index }}) {
        modal{{ forloop.index }}.style.display = "none";
      }
    }
  {% endfor %}
</script>

<!-- <div class="container">
    <div class="post-list" itemscope itemtype="http://schema.org/Blog">
        {% for area in site.areas %}
            {% include areacard1.html %}
        {% endfor %}
    </div>
</div>

<link href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.4/css/lightbox.min.css" rel="stylesheet" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.4/js/lightbox.min.js"></script> -->

---

<br/>

## News

<!-- Elfsight Instagram Feed | Untitled Instagram Feed -->
<script src="https://elfsightcdn.com/platform.js" async></script>
<div class="elfsight-app-a4477114-d6a2-4202-93f9-b6165dd7def0" data-elfsight-app-lazy></div>
