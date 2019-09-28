---
layout: archive
permalink: /credit/
title: "Credit"
author_profile: true
---

클래식 메이트는 서울대학교 UX랩과 클래식 공연 기획사 크레디아가 공동으로 개발한 스마트 스피커 서비스입니다. 

모든 음원은 크레디아가 제공합니다.

<figure>
  <img src="{{ '/assets/images/land-logo.png' | relative_url }}" alt="fork Minimal Mistakes" width="100">
</figure>

<figure>
  <img src="{{ '/assets/images/credia.png' | relative_url }}" alt="fork Minimal Mistakes" width="100">
</figure>

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
