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

## Research
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



<div class="container">
    <div class="carousel">
        <input type="radio" name="slides" checked="checked" id="slide-1">
        <input type="radio" name="slides" id="slide-2">
        <input type="radio" name="slides" id="slide-3">
        <input type="radio" name="slides" id="slide-4">
        <input type="radio" name="slides" id="slide-5">
        <input type="radio" name="slides" id="slide-6">
        <ul class="carousel__slides">
            <li class="carousel__slide">
                <figure>
                    <div>
                      <img src="{{ site.url }}{{ site.baseurl }}/_img/main/Penguins.jpg" width=100%>
                    </div>
                    <figcaption>
                        Penguins.
                        <span class="credit">001</span>
                    </figcaption>
                </figure>
            </li>
            <li class="carousel__slide">
                <figure>
                    <div>
                      <img src="{{ site.url }}{{ site.baseurl }}/_img/main/Desert.jpg" width=100%>
                    </div>
                    <figcaption>
                        Desert.
                        <span class="credit">002</span>                            
                    </figcaption>
                </figure>
            </li>
            <li class="carousel__slide">
                <figure>
                    <div>
                      <img src="{{ site.url }}{{ site.baseurl }}/_img/main/Jellyfish.jpg" width=100%>
                    </div>
                    <figcaption>
                        Jellyfish.
                        <span class="credit">003</span>                            
                    </figcaption>
                </figure>
            </li>
        <ul class="carousel__thumbnails">
            <li>
                <label for="slide-1"><img src="{{ site.url }}{{ site.baseurl }}/_img/main/Penguins.jpg"></label>
            </li>
            <li>
                <label for="slide-2"><img src="{{ site.url }}{{ site.baseurl }}/_img/main/Desert.jpg"></label>
            </li>
            <li>
                <label for="slide-3"><img src="{{ site.url }}{{ site.baseurl }}/_img/main/Jellyfish.jpg"></label>
            </li>
        </ul>
    </div>
</div>
