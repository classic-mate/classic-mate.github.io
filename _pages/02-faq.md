---
layout: archive
permalink: /faq/
title: "자주 묻는 질문"
author_profile: true
---

**1. 클래식 메이트, 어떻게 시작하나요?**

가지고 계신 [<mark>구글 스마트스피커</mark>](https://store.google.com/kr/magazine/compare_nest_speakers_displays){:target="_blank"}에 ‘Ok Google, 클래식 메이트에게 말하기’ 를 시도해 보세요.

**2. 구글 스마트스피커에서만 가능한가요?**

가지고 계신 <mark>휴대전화에 구글 어시스턴트 앱 설치 후</mark> ‘클래식 메이트에게 말하기’ 를 시도해 보세요.

**3. 토니는 누구인가요?**

여러분이 AI를 더욱 즐겁게 이용할 수 있도록 준비했답니다. 클래식 음악을 설명해 주는 캐릭터이고, 작곡가 ‘안토니오 비발디’에서 따온 이름이라 토니랍니다. 어디선가 들어본 목소리인가요?
[바이올리니스트 대니 구](http://www.credia.co.kr/board/?db=gallery_2&no=124&mari_mode=view@view){:target="_blank"}의 실제 목소리를 합성해서 제작 했습니다.  


**4. 스마트스피커가 멈춘 것 같아요...**

가끔 사용 중 스마트스피커가 멈추는 경우가 있답니다. 멈췄던 스피커는 스스로 다시 켜지니, 잠시 기다렸다가 다시 클래식 메이트를 불러주세요.  

**5. 알람처럼 매일 정해진 시간에 듣고 싶어요**

구글홈 루틴 설정을 사용해보세요!
루틴 설정하는 방법은 **[120% 활용하기](https://classic-mate.github.io/about/) 탭**에서 상세히 알려드릴게요.

**6. 어제와 오늘의 추천곡, 다시 듣고 싶어요**

클래식 메이트를 부르고 **“어제(이저) 음악 틀어줘”** 혹은 **“오늘 음악 다시”**라고 말해보세요. <br>
내일의 추천곡을 미리 듣고 싶으면 **“내일(다음) 음악 틀어줘”**라고 말해주세요!

**7. 지금까지 들었던 곡을 알 수는 없나요?**

첫날 들려 드린 음악부터 매일 업데이트 할 예정이에요. 추후에 공지할테니 이곳에서 확인해 주세요! 

**8. 계정 연동이 안되는데...**

구글홈 보이스 매치를 설정해보세요! 보이스 매치 설정 방법은 [이곳](https://support.google.com/googlenest/answer/7342711?hl=ko){:target="_blank"}에서 확인하실 수 있습니다.
클래식 메이트를 처음 사용하실 때 계정 정보 사용에 꼭 동의를 해주셔야 합니다!

**9. 사용할 때마다 새로 계정을 연동하래요**

[구글 내 활동](https://myactivity.google.com/myactivity?hl=ko){:target="_blank"}에서 [활동 제어]에 들어가세요. [웹 및 앱 활동] 아래의 두 가지 항목을 모두 체크해주시면 됩니다!

**10. 계정이 리셋됐는데, 이어서 듣고 싶어요**

죄송해요. 리셋된 계정은 복구가 어렵답니다.

**다른 문제가 있나요?**

<info@credia.co.kr>로 문의해주세요


{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
