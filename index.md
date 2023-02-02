---
#
# You don't need to edit this file, it's empty on purpose.
# Edit sleeks's default layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: default
title: 건축도시공간연구실
secondtitle: Lab for Architectural & Urban Space
---

건축도시공간연구실(LAUS)은 건축과 도시공간을 분석하여, 더욱 인간적이고 합리적인 공간이 될 수 있는 방법을 연구하고 있습니다.

1999년 설립 이후 현재에 이르기까지 공간계획과 기획에 관련한 여러 연구를 수행하고 있습니다.

## Research Areas
<div class="container">
    <div class="post-list" itemscope="" itemtype="http://schema.org/Blog">
    {% assign areas = site.areas %} 
    {% assign sorted_areas = areas | sort: "importance" %} 
    {% for area in sorted_areas %}
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


<div class="news">
  <a href="/news"><h2>News</h2></a>
  {% if site.news  %}
    <div class="table-responsive">
      <table class="table table-sm table-borderless">
      {% assign news = site.news | where: "on-home", "true" | reverse %}
      {% for item in news limit: site.news_limit %}
        <tr>
          <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
          <td>
            {% if item.inline %}
              {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
            {% else %}
              <a class="news-title" href="{{ item.permalink | relative_url }}">{{ item.title | remove: '<p>' | remove: '</p>' | replace: '<br/>', " " }}</a><br/>
              <div class="summary">
              {{ item.content | remove: '<p>' | remove: '</p>' | emojify | truncatewords:50 }}
              </div>
            {% endif %}
          </td>
        </tr>
      {% endfor %}
      </table>
    </div>
  {% else %}
    <p>No news so far...</p>
  {% endif %}
</div>
