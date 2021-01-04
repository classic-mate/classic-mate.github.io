---
layout: archive
permalink: /credit/
title: "Credit"
author_profile: true
---

<!-- 클래식 메이트는 서울대학교 UX랩과 클래식 공연 기획사 크레디아가 공동으로 개발한 스마트 스피커 서비스입니다. 

모든 음원은 크레디아가 제공합니다. -->

<!-- <figure>
  <center><img src="{{ '/assets/images/land-logo.png' | relative_url }}" alt="fork Minimal Mistakes" width="100"></center>
</figure>
 -->
<!-- 
> 서울대학교 UX 랩 :
> 대화형 서비스에 최적화된 대화 플로우 디자인 및 사용자 중심적인 요소에 기반한 서비스 개발

> 크레디아 : 
> 클래식 음악의 대중화에 맞춘 전문적인 콘텐츠 기획 및 양질의 음원 제공

 -->
큐레이션 : 디토디지털오디세이 <br>
서비스 기획 및 개발 : 서울대학교 UX랩 <br>
음원 제공: <br>
&nbsp;&nbsp;&nbsp;&nbsp; 크레디아뮤직앤아티스트 [http://www.credia.co.kr/](http://www.credia.co.kr/){:target="_blank"} <br>
&nbsp;&nbsp;&nbsp;&nbsp; 코리안심포니오케스트라 [http://koreansymphony.com/](http://koreansymphony.com/){:target="_blank"}

---

**디토디지털오디세이**는 클래식 공연 기획사 크레디아의 콘텐츠/퍼블리싱 컴퍼니입니다. 음원, 영상, 도서 등 다양한 콘텐츠 기획/제작과 저작권 관리를 담당합니다. 멜론, 지니, FLO 등 국내 주요 플랫폼 뿐만 아니라 스포티파이, 유튜브 뮤직, 애플 뮤직, 아마존 등 해외에도 음원과 영상을 공급하고 있습니다. 새로운 기술과 협력하여 음악의 즐거움이 오래, 널리 전달되도록 하겠습니다.

**크레디아뮤직앤아티스트**는 1994년 설립된 이후, 클래식 음악을 중심으로 세계 정상급 연주자의 한국 공연을 기획, 제작해 온 클래식 공연기획사입니다. 전국 공연장과 페스티벌에 양질의 클래식 공연을 제공하고 있으며, 또한 국제적인 경쟁력을 가진 한국 연주자의 매니지먼트를 통해 국내는 물론 해외무대 진출을 적극 지원합니다.

**서울대학교 UX랩**은 다양한 정보 미디어와 기술에 둘러싸인 사용자를 관찰하기 위해서 창의적이고 사회문화적인 접근을 추구합니다. 창조적이고 순발력있는 연구 방법을 통해 보다 통찰력있는 이용 경험 관찰 및 행동 패턴 분석, 사용자 니즈 도출을 수행하고 있습니다.

특별히, 오케스트라 음악 음원 제공에 협조해 주신 **코리안심포니오케스트라**에 감사 인사 드립니다. 

<!-- <figure>
  <center><img src="{{ '/assets/images/credia.png' | relative_url }}" alt="fork Minimal Mistakes" width="100"></center>
</figure> -->

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
