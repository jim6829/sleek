---
layout: post
title: "MakeyStickey"
summary: 모션 인식 게임 컨트롤러
featured-img: makeystickey/hero
unit: team
positions: [Developer]
categories: [Game Controller, Tangible Interface, Prototype, Software Engineering, Arduino]
categories-card: [Game Controller]
publish: y
---

# "모션 인식 게임 컨트롤러"


![MakeyStickey](/assets/img/posts/makeystickey/controller.jpg#center)
## Abstract
MakeyStickey는 아케이드 게임 [Stickman Hook](https://poki.com/en/g/stickman-hook)을 모션 기반으로 즐길 수 있게 만들어주는 게임 컨트롤러이다. 키보드의 스페이스바만 사용하는 기존의 정적인 조작 방식을 물리적인 몸동작으로 변환함으로써 생동감 넘치는 게임 경험을 유도한다. 플레이어는 마블 코믹스의 대표 캐릭터 스파이더맨(Spiderman)의 제스처를 취함에 따라 게임을 진행하게 된다.

***

## Video
<div class="video-container">
	<iframe class="video-frame" src="https://www.youtube.com/embed/3zfINlh1Wcs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

***

## Interface

### Game: Stickman Hook
![Stickman Hook](/assets/img/posts/makeystickey/stickman_hook.jpg#center)
Stickman Hook은 아케이드 장르의 게임으로 키(스페이스바 또는 마우스 왼쪽 버튼)를 눌러 동그라미의 중심축으로 뿜어낸 줄과 흰 벽에 달린 뜀판을 이용해 앞뒤로 이동하며 피니시 라인까지 도달해야 하는 게임이다. 하나의 버튼만을 사용하는 단순한 인터랙션이 특징이며 속도, 길이, 관성, 탄성 등을 고려해 타이밍을 맞춰야 한다.

### Controller: MakeyStickey
![Spiderman](/assets/img/posts/makeystickey/spiderman.gif#center)
MakeyStickey는 마블 코믹스의 대표적인 캐릭터 스파이더맨에서 모티브를 따온 제스처 인터페이스이다. 사용자는 스파이더맨이 거미줄을 뿜어내는 팔동작, 손동작을 그대로 재현함으로써 게임 속 Stickman의 줄을 조작하게 된다.

![Flow](/assets/img/posts/makeystickey/flow.png#center)
컨트롤러는 팔 토시와 팔뚝의 아대로 구성된다. 손가락이 펴져 있고 팔이 굽혀진 상태가 원위치이며, 이때 팔을 피면서 손가락을 접으면 Stickman의 줄이 발사된다. 이후 팔을 다시 굽히거나 손가락을 피면 줄이 회수된다. 선행 조건이 하나라도 맞지 않으면 줄이 발사되지 않는다.

전반적인 구조는 토시 내부에 아두이노(Arduino)의 일종인 메이키메이키(MaKeyMaKey)가 위치한 형태이다. 먼저 팔뚝의 아대와 팔의 접촉 여부에 따라 팔의 동작을 감지하고, 이후 손가락과 거미의 접촉 여부에 따라 손의 동작을 감지한다.