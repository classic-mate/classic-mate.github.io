---
layout: archive
permalink: /about/
title: "120% 활용하기"
author_profile: true
---

**클래식 메이트의 추가 기능을 알려드립니다**

<!--
**랜덤 추천받기**

“새로운 곡 없나?” 
오늘의 추천곡과 상관 없이 새로운 음악이 듣고 싶을 때는 **“Ok Google, 클래식 메이트한테 랜덤추천받기”**라고 말해보세요. <br>
오늘의 음악을 듣다가도 **“Ok Google, 랜덤곡 들려줘”**라고 하면 새로운 음악을 소개해드린답니다!
---
-->
**루틴 설정하기**

“정해진 시간에 클래식 메이트를 만나고 싶다.”<br>
**구글홈 루틴 설정**을 이용하면 정해진 시간에 클래식 메이트가 찾아와요!


<iframe width="560" height="315" src="https://www.youtube.com/embed/-g97MQl6RXw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

1. 루틴 클릭
2. 루틴 관리 클릭
3. 루틴 추가 클릭
4. 원하는 명령어 및 날짜 설정, 적용할 스피커 선택
5. 작업 추가 클릭하고 "클래식 메이트한테 말하기" 입력
6. 저장!

---

**클래식 메이트의 공연 추천**

오늘의 음악 감상이 끝나면 토니가 클래식 공연과 영상을 추천해 주기도 한답니다. <br>
깜짝 선물처럼 찾아오는 공연 추천을 놓치지 마세요!<br><br>


**[5G로 만나는 클래식! 온:클래식](https://bit.ly/38GIlH8)**  <br>
공연도 온라인 실감영상으로! 모든 팬이 'R석'의 즐거움을! <br>
- 연주, 지휘, 해설까지 초 직관뷰로 공연의 생생함 완벽 전달 <br>
- 세계 최초 5GX멀티뷰 오케스트라 공연, 웨이브와 B tv 단독 제공 <br>

클래식 공연 '언택트 관람시대'를 위해 제작한 실감 영상을 만나보세요. <br>
**하나의 공연을 6개의 화면에서 선택**해서 감상할 수 있습니다. 선택 화면에 따라 특정 연주자의 음을 강조해 들을 수 있습니다. 원하는 화면만 모아볼 수 있고, 원하는 부분을 최대 4배까지 확대해서 볼 수도 있답니다. 화면 별로 VOD 감상도 가능합니다. <br><br>


**크레디아 클래식 클럽 2021** <br>
가격은 낮추고 감동은 올리고, 당신의 1년이 클래식해 집니다. <br>
믿고 듣는 크레디아의 대표 아티스트와 쟁쟁한 해설자가 함께하는 마티네 공연을 소개합니다. 한달에 한번, 2021년 연간 총 10회 롯데콘서트홀에서 만나보세요. 정상급 연주자의 연주와 명망 높은 해설을 합리적인 가격으로 감상할 수 있습니다. 

![Credia Classic Club](https://classic-mate.github.io/assets/images/crediaclassicclub.jpeg)



{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  {% for post in year.items %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
