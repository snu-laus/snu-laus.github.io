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

서울대학교 건축도시공간연구실(LAUS)은 1999년 설립 이래 [도시, 주거, 건축](https://snu-primo.hosted.exlibrisgroup.com/permalink/f/177n5ka/82SNU_INST21879086720002591) 분야의 연구를 이어오고 있습니다.

LAUS의 연구 질문은 하나로 모입니다. **한국의 도시와 주거는 어떤 형태로 만들어졌고, 그 형태는 우리의 삶에 어떻게 영향을 미치는가?** 아파트 단지, 신도시, 서울 도심의 형태를 분석하고, 그 형태를 만든 제도와 정책, 그리고 그 안에서 살아가는 사람들의 이동과 일상을 연결하여 이해합니다.

현재 LAUS의 연구는 크게 두 갈래로 진행됩니다.

#### 🟦 도시형태 연구

**형태와 정책**: 제도는 어떤 공간을 만들었나. 도시설계 담론에 따른 신도시 블록 크기의 변화, 길 단위 용도혼합의 현황, 서울 도심재개발 정책의 변천을 통해 정책과 형태의 관계를 추적합니다.

**공간과 수치**: 밀도와 거리만으로는 도시공간의 형태를 기술할 수 없습니다. GIS와 시공간 데이터, 휴대폰 위치기록, 건축행정데이터, 기계학습과 대규모 언어모델을 결합해 그 형태를 측정하는 방법 자체를 연구합니다.

#### 🟢 사회적 도시건축

**도시와 주거**: 한국의 지배적 주거 모델인 아파트 단지를 들여다봅니다. 단지계획과 단지 내 상가의 변천, 아파트와 비아파트 거주자의 생활공간 차이를 실증하고, 결국 우리는 어떻게 모여 살아야 하는가를 묻습니다.

**고령화, 쇠퇴, 정비**: 분석을 설계와 정책으로 되돌립니다. 초고령사회의 근린환경과 공공공간, 저층주거지의 지속가능한 재정비, 빈집 문제에서 출발해 우리 도시건축의 사회적 이슈를 탐구합니다.

---

The Lab for Architectural and Urban Space (LAUS) has studied [cities, housing, and architecture](https://snu-primo.hosted.exlibrisgroup.com/permalink/f/177n5ka/82SNU_INST21879086720002591) since its founding in 1999, in the Department of Architecture and Architectural Engineering at Seoul National University.

The research questions at LAUS converge on one: **how did Korea's cities and housing come to take their present form, and how does that form shape the way we live?** We analyze the form of apartment complexes, new towns, and central Seoul, and connect it to the institutions and policies that produced it, and to the movement and everyday life of the people within it.

Our research currently follows two lines.

#### 🔵 Urban Form Studies

**Form & Policy**: What kind of space did institutions build? We trace the relationship between policy and form through changing block sizes in new towns shaped by urban design discourse, the present state of street-level land use mix, and the evolution of downtown redevelopment policy in Seoul.

**Space & Measure**: Density and distance alone cannot describe the form of urban space. We study the measurement of that form itself, combining GIS and spatiotemporal data, mobile phone location histories, building administrative records, machine learning, and large language models.

#### 🟢 Social Architecture and Urbanism

**City & Housing**: We examine the apartment complex, Korea's dominant housing model: how the planning of complexes and their internal retail have evolved, how activity spaces differ between apartment and non-apartment residents, and ultimately how we should live together.

**Aging, Shrinkage, & Renewal**: We return analysis to design and policy. Beginning from neighborhood environments and public space for a super-aged society, the sustainable renewal of low-rise neighborhoods, and the problem of vacant houses, we explore the social questions facing architecture and urbanism in Korea.

---

대학원 진학이나 연구실 참여에 관심이 있으신가요? [안내 페이지](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284)를 먼저 확인해 주세요.

학부연구생도 모집하고 있습니다. 자세한 내용은 [모집 공고](https://snu-laus.notion.site/2ab32921929280578f53ed18d64a12da?pvs=74)에 있습니다.

If you are interested in joining LAUS as a graduate student, please start with [this guide page](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284).

We are also recruiting undergraduate research assistants. See the [call for applications](https://snu-laus.notion.site/2ab32921929280578f53ed18d64a12da?pvs=74) for details.

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
