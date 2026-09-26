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

LAUS의 연구는 하나의 질문으로 모입니다. **한국의 도시와 주거는 어떤 형태로 만들어졌고, 그 형태는 우리의 삶에 어떤 영향을 미치는가?** 아파트 단지, 신도시, 서울 역사도심처럼 한국 도시를 특징짓는 공간형태를 분석하고, 그 형태를 만들어 낸 제도·정책과 그 속에서 이루어지는 사람들의 생활을 함께 탐구합니다.

현재 LAUS의 연구는 크게 두 주제로 나뉩니다.

#### 🟦 도시형태 연구

**형태와 정책**: 제도는 어떤 공간을 만들었는가? 도시건축 제도, 개념, 담론이 한국 도시에 만들어 낸 공간형태를 추적합니다.

**공간과 측정**: 도시공간의 형태는 어떻게 기술할 수 있는가? 건축물 데이터, 가로 이미지, 휴대전화 데이터 등을 GIS와 인공지능 기법으로 분석하며, 형태를 측정하는 방법 자체를 연구합니다.

#### 🟢 사회적 도시건축

**도시와 주거**: 한국의 대표적 주거 모델인 아파트 단지를 들여다봅니다. 단지계획과 단지 내 상가의 변천을 추적하고, 아파트와 비아파트 거주자의 생활공간 차이를 실증하며, 궁극적으로 우리는 어떻게 모여 살아야 하는가를 묻습니다.

**고령화, 쇠퇴, 정비**: 분석의 성과를 설계와 정책으로 되돌립니다. 초고령사회의 근린환경과 공공공간, 저층주거지의 지속가능한 재정비, 빈집 문제를 출발점으로 우리 도시건축이 마주한 사회적 과제에 해법을 제시합니다.

---

Since its founding in 1999 in the Department of Architecture and Architectural Engineering at Seoul National University, the Lab for Architectural and Urban Space (LAUS) has carried out research on [cities, housing, and architecture](https://snu-primo.hosted.exlibrisgroup.com/permalink/f/177n5ka/82SNU_INST21879086720002591).

Our research converges on a single question: **How did Korea's cities and housing take shape, and how does that form affect the way we live?** We analyze the spatial forms that characterize Korean cities, such as apartment complexes, new towns, and Seoul's historic core, and investigate them together with the institutions and policies that produced them and the everyday lives that unfold within them.

Our research currently falls under two themes.

#### 🟦 Urban Form Studies

**Form & Policy**: What kind of space have institutions created? We trace the spatial forms that urban and architectural regulations, concepts, and discourses have produced in Korean cities.

**Space & Measure**: How can the form of urban space be described? Analyzing building data, street-view imagery, mobile phone data, and more with GIS and AI techniques, we study the methods of measuring form itself.

#### 🟢 Social Architecture and Urbanism

**City & Housing**: We examine the apartment complex, Korea's predominant housing model. We trace how complex planning and on-site retail have evolved, empirically compare the activity spaces of apartment and non-apartment residents, and ultimately ask how we should live together.

**Aging, Shrinkage, & Renewal**: We bring our analysis back to design and policy. Starting from neighborhood environments and public space in a super-aged society, the sustainable renewal of low-rise residential areas, and vacant housing, we propose solutions to the social challenges facing architecture and urbanism in Korea.

---

대학원 진학이나 연구실 참여에 관심이 있으신가요? [안내 페이지](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284)를 먼저 확인해 주세요.

학부연구생도 모집하고 있습니다. 자세한 내용은 [모집 공고](https://snu-laus.notion.site/2ab32921929280578f53ed18d64a12da?pvs=74)를 참고해 주세요.

Interested in graduate study or joining the lab? Please start with [this guide page](https://bumjoon.notion.site/Join-the-Lab-5e1fd035bf0d40828e356a97fa2f4284).

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
