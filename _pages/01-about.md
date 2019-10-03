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

1. 루틴을 클릭
2. 루틴 관리를 클릭
3. 추가 버튼을 클릭
4. 명령어 추가를 클릭
5. 클래식 메이트 입력 후 저장
6. 시간 및 날짜 설정을 클릭
7. 요일, 시간, 적용할 스피커를 선택
8. 작업 추가를 클릭
9. 클래식 메이트한테 말하기를 입력 후 추가를 클릭

---

**클래식 메이트의 공연 추천**

음악 감상이 끝나고 클래식 메이트가 공연 추천을 해주기도 한답니다. 깜짝 선물처럼 찾아오는 공연 추천을 놓치지 마세요!
아래 올해의 추천 공연도 확인해보세요!

* 2019년 12월 01일
[지용 피아노 리사이틀](http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010644)

<!-- <figure>
  <img src="{{ '/assets/images/concert1.jpg' | http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010644 }}" alt="fork Minimal Mistakes">
</figure> -->

* 2019년 12월 29일
[사라 장 바이올린 리사이틀](http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010938)

<!-- <figure>
  <img src="{{ '/assets/images/concert2.jpg' | http://ticket.interpark.com/Ticket/Goods/GoodsInfo.asp?GoodsCode=19010938 }}" alt="fork Minimal Mistakes">
</figure>
 -->
{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  {% for post in year.items %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}