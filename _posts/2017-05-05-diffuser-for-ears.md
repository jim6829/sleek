---
layout: post
title: "Diffuser for Ears"
summary: 소리를 담은 디퓨저
featured-img: diffuser-for-ears/hero
unit: personal
positions: [Developer, Designer]
categories: [Interactive Media, Tangible Interface, Product Design, Software Engineering, Arduino]
categories-card: [Interactive Media]
publish: y
---

# "소리를 담은 디퓨저"

![Diffuser for Ears](/assets/img/posts/diffuser-for-ears/grass.jpg#center)
## Abstract
Diffuser for Ears는 주변 환경의 소리([Soundscape](https://en.wikipedia.org/wiki/Soundscape))를 설계할 수 있는 디퓨저이다. 각 디퓨저는 고유의 소리를 담고 있으며 뚜껑을 열면 소리가 난다. 사용자는 마치 조향을 하듯 디퓨저들을 조합해 원하는 사운드스케이프 장면을 만들 수 있다.

이 작업은 이후 [Ambience](/ambience)라는 데스크탑 앱으로 확장되었다.

***

## Video
<div class="video-container">
	<iframe class="video-frame" src="https://www.youtube.com/embed/mInbQGadB2w" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

***

## Background
오늘날 사람들의 생활공간은 제한적이다. 금요일까지 각종 과업에 시달리고 주말에 밀린 잠을 자면 어느새 일주일이 끝나고는 한다. 결국 일상 속에서 여가와 휴식을 취할 수 있는 공간은 집이 거의 유일하다. 이때 집이라는 한정된 공간을 보다 넓은 환경으로 확장할 수 있다면 현대인들의 심신을 효과적으로 환기할 수 있다고 보았다.

![Little Prince](/assets/img/posts/ambience/box.jpg#center)

소리는 인간을 상상하게 만든다. 시지각과 달리 청각은 명징함이 덜하면서 동시에 상상의 여지를 남긴다. 이러한 청각의 유연함은 어린왕자의 상자와 같은 상상의 창구로 작용한다. 공간의 확장에 사운드스케이프 개념을 도입한 이유이다.

***

## Design
![Diffuser for Ears](/assets/img/posts/diffuser-for-ears/shots.png#center)
디퓨저는 총 5개로 구성되며 각각 풀, 바다, 모닥불, 비, 그리고 새의 소리를 담고 있다.

작품 내부에는 아두이노([Arduino](https://www.arduino.cc))를 비롯한 전기적 장치가 위치한다. 아두이노는 압력센서를 통해 디퓨저 뚜껑의 움직임을 감지한 뒤 프로세싱([Processing](https://processing.org))과 통신하여 소리를 제어한다.