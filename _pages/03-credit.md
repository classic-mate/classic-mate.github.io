---
layout: archive
permalink: /credit/
title: "Credit"
author_profile: true
---

<!-- 클래식 메이트는 서울대학교 UX랩과 클래식 공연 기획사 크레디아가 공동으로 개발한 스마트 스피커 서비스입니다. 

모든 음원은 크레디아가 제공합니다. -->

<figure>
  <img src="{{ '/assets/images/land-logo.png' | relative_url }}" alt="fork Minimal Mistakes" width="50">
</figure>

<!-- - 서울대학교 UX랩 :  -->

대화형 서비스에 최적화된 대화 플로우 디자인 및 사용자 중심적인 요소에 기반한 서비스 개발

<figure>
  <img src="{{ '/assets/images/credia.png' | relative_url }}" alt="fork Minimal Mistakes" width="50">
</figure>

<!-- - 크레디아 :  -->

클래식 음악의 대중화에 맞춘 전문적인 콘텐츠 기획 및 양질의 음원 제공



{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
