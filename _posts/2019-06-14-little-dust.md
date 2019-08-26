---
layout: post
title: "Little Dust (작은 먼지)"
summary: 관객과 함께 완성되는 책
featured-img: little-dust/hero
unit: team
positions: [Developer]
categories: [Interactive Media, Tangible Interface, Software Engineering, Arduino]
categories-card: [Interactive Media]
publish: y
---

# "관객과 함께 완성되는 책"


![Little Dust](/assets/img/posts/little-dust/front.jpg#center)
## Abstract
작은 먼지는 “별똥별 이야기”라는 책을 인터랙티브 미디어로 풀어낸 작업이다. 기존의 정적인 매체로서의 책에 상호작용성을 더함으로써 독자가 책을 읽는 경험을 극대화한다. 관객은 이야기와 유기적으로 연결된 행위를 수행함에 따라 책을 진행시키게 되며 책을 은유하는 디오라마의 시각적, 청각적 변화를 통해 이야기를 입체적으로 감상하게 된다.

***

## Video
<div class="video-container">
	<iframe class="video-frame" src="https://www.youtube.com/embed/a24myr6ZH2k" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

***

## Story
```
‘반짝’

커다랗고 머나먼 우주,
한 소행성에서 떨어져 나온 작은 먼지가 있었다.
작은 먼지는 우주를 여행하고 있다.

사실, 작은 먼지는	
오랫동안 홀로 여행하느라
조금 지치고 외로웠다.

어디선가 작은 먼지를 잡아당겼다.
여행의 마지막은 푸른 빛이 감도는 행성이었다.
밤 공기가 차가워질 때
작은 먼지는 뜨겁게 빛이 나기 시작했다.

속삭임이 들렸다.
작은 먼지는 귀를 귀울였다.
“별똥별아, 나의 소원을 들어줘.”

누군가 작은 먼지에게 소원을 빌었다.
그 사람은 작은 먼지에게
‘별똥별’이라는 이름을 붙여주었다.

별똥별은
아름다운 이름과
누군가의 소중한 소원을 안고
여행을 마무리한다.

‘반짝’


커다란 우주의 작은 먼지에 불과한 우리도
누군가에게는 별똥별 같은 존재입니다.
```

***

## Structure
![Little Dust](/assets/img/posts/little-dust/overall_structure.png#center)
![Little Dust](/assets/img/posts/little-dust/side_view.jpg#center)
작품의 전반적인 구성은 작은 탁자에 올라갈 수 있는 크기의 디오라마와 이 위에 이미지를 투사하는 프로젝터의 조합이다. 디오라마는 책의 세계를 대변하는 만큼 순수한 흰색 종이로 만들어진 페이퍼 아트 형태이며, 프로젝터는 종이 위에 우주와 글을 비추게 된다.

작품 내부에는 아두이노([Arduino](https://www.arduino.cc))를 비롯한 전기적 장치가 위치한다. 아두이노는 디오라마의 조명을 제어하고 여러 센서를 통해 관객의 행위를 감지하며 프로세싱([Processing](https://processing.org))과의 통신을 통해 디오라마에 투사하는 이미지를 제어한다.