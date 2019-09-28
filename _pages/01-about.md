---
layout: archive
permalink: /about/
title: "120% 활용하기"
author_profile: true
---

**랜덤 추천받기**

스테이지에 상관 없이 새로운 음악이 듣고 싶을 때는 “Ok Google, 클래식 메이트한테 랜덤추천받기”라고 말해보세요. 어쩌면 당신의 인생 음악을 찾게 될 수도 있어요!

---

**루틴 설정하기**

구글홈 루틴 설정을 이용하시면 정해진 시간에 클래식 메이트가 찾아와요!

---

**클래식 메이트의 공연 추천**

클래식의 매력에 더욱 빠져보세요!

<figure>
  <img src="{{ '/assets/images/concert1.jpg' | http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010644 }}" alt="fork Minimal Mistakes">
</figure>

<figure>
  <img src="{{ '/assets/images/concert2.jpg' | http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010938 }}" alt="fork Minimal Mistakes">
</figure>

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  {% for post in year.items %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}