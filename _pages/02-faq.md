---
layout: archive
permalink: /faq/
title: "자주묻는 질문"
author_profile: true
---

**1. 알람처럼 매일 정해진 시간에 듣고 싶어요**

구글홈 루틴 설정을 사용해보세요!
루틴 설정하는 방법은 [[120% 활용하기]](https://classic-mate.github.io/about/) 탭에서 상세히 알려드릴게요.

**2. 어제와 오늘의 추천곡, 다시 듣고 싶어요**

클래식 메이트를 부르고 “어제 음악 틀어줘”
혹은 “오늘 음악 다시”라고 말해보세요. 내일의 추천곡을 미리 듣고 싶으면 “내일 음악 틀어줘”라고 말해주세요!

**3. 계정 연동이 안돼요**

구글홈 보이스 매치를 설정해보세요! 보이스 매치 설정 방법은 [이곳](https://support.google.com/googlenest/answer/7342711?hl=ko)에서 확인하실 수 있습니다.
클래식 메이트를 처음 사용하실 때 계정 정보 사용에 꼭 동의를 해주셔야 합니다!

**4. 계정이 리셋됐는데, 이어서 듣고 싶어요**

죄송해요. 리셋된 계정은 복구가 어렵답니다.

**다른 문제가 있나요?**

클래식메이트의 카카오톡 플러스 친구에게 문의해주세요! 
(ID: 클래식메이트)

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}