---
layout: archive
permalink: /credit/
title: "Credit"
author_profile: true
---

클래식 메이트는 서울대학교 UX랩과 클래식 공연 기획사 크레디아가 공동으로 개발한 스마트 스피커 서비스입니다. 

모든 음원은 크레디아가 제공합니다.

<figure>
  <center><img src="{{ '/assets/images/land-logo.png' | relative_url }}" alt="fork Minimal Mistakes" width="100"></center>
</figure>

<figure>
  <center><img src="https://www.google.com/url?sa=i&source=images&cd=&ved=2ahUKEwjPpqXt5PPkAhWbKqYKHYWIDzYQjRx6BAgBEAQ&url=http%3A%2F%2Fwww.credia.co.kr%2F&psig=AOvVaw1Iq5P8TitOjlbYMn3Ay4RS&ust=1569769399281847" width="100"></center>
</figure>

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
