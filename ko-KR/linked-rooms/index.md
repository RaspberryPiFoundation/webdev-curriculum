---
제목: 연결된 방
난이도: HTML & CSS 2
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...
 
# 소개 {.intro}

이 프로젝트에선 각자 HTML로 꾸민 연결된 여러 방들을 만들 것입니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ba5d27ec68?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="rooms-hall-finished.png">
</div>

__설명__: 문을 클릭하여 방 사이를 오가세요.

# 1 단계: 같은 프로젝트내에서 다른 웹페이지 링크 해 넣기 {.activity}

웹 프로젝트는 여러 개의 링크된 HTML 파일들로 만들어질 수 있습니다. 

## 단계별 체크리스트 { .check}

+ 이 트링켓을 열어주세요: <a href="http://jumpto.cc/web-rooms" target="_blank">jumpto.cc/web-rooms</a>. 혹은 온라인으로 읽고 있다면  아래의 embedded 된 트링켓을 사용할 수 있습니다

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ef608f0733" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 트링켓이 자동 실행되면 현관에 있는 걸 볼 수 있습니다:

	![screenshot](rooms-hall-start.png)

+ 트링켓의 파일 탭 리스트를 보세요. `tvroom.html`을 찾고 클릭하세요.

	![screenshot](rooms-tvroom-html.png)

	같은 프로젝트의 다른 HTML 파일입니다


+ `tvroom.html` 으로 가려면 `index.html`에 링크를 더해야 합니다. 

	강조된 코드를  `<div>` 안에 class `room`과 함께 넣으세요: 

	![screenshot](rooms-link-tvroom.png)

+  __TV Room__ 링크를 클릭해서 `tvroom.html` 페이지가 보이는지 확인해보세요.

	`tvroom.html` 에는 이 페이지의 레이아웃을 결정하는 고유의 `tvroom.css` 스타일 파일이 있다는 데도 주목해주세요. 

	![screenshot](rooms-tvroom-unstyled.png)

	
##도전과제: 다른 링크 더하기 {.challenge}

 `<a>` 링크를 `tvroom.html` 웹페이지에 더해 `index.html`라고 불리는 현관 페이지로 돌아가게 만드세요. 링크 텍스트는 'Hall' 이어야 합니다.

TV Room webpage 에 이런 클릭 가능한 링크가 생겨야 합니다:

![screenshot](rooms-hall-link.png)

이 코드를 시험해보는 걸 잊지 마세요. 현관에서 TV Room으로, 그리고 다시 현관으로 링크를 클릭해서 오 다닐 수 있어야 합니다.


## 프로젝트를 저장하세요 {.save}

# 2 단계: 다른 방 더하기 {.activity}

이제  __Games Room__을 추가해 넣읍시다. 

+ 페이지 더하기 __+__ 버튼을 넣으세요:

	![screenshot](rooms-add-page.png)

	페이지 이름을 `gamesroom.html` 으로 넣으세요:

  	![screenshot](rooms-games-html.png)

+ __Games Room__ 의 HTML은  `tvroom.html`과 매우 비슷함으로  __복사해서__  `gamesroom.html`으로  __붙여 넣으세요__.
	
	다음 강조된 아이템을 수정해서 TV 대신 Games라고 나오게 만드세요:

	![screenshot](images/rooms-games-html2.png)	

+ 이제 `gamesroom.html` 은 아직 존재하지 않는 `gamesroom.css`를 사용합니다. 

	페이지 더하기 __+__버튼을 눌러서  `gamesroom.css` 를 만드세요. 


+  __Games Room__ 의 CSS는 `tvroom.css` 와 매우 비슷함으로  __복사해서__ `gamesroom.css`로  __붙여 넣으세요__.

	![screenshot](rooms-add-games-css.png)

+ 현관에서 Games Room으로 가는 링크를 더하세요:

	![screenshot](rooms-hall-games.png)

+ Games Room 링크를 클릭해서 프로젝트를 시험해보세요.

	__Games Room__ 은 이렇게 보일 것입니다:

	![screenshot](rooms-games-before.png)

	별로 재미있어 보이는 페이지가 아니지만 다음 도전과제로 고칠 수 있습니다.

## 프로젝트를 저장하세요 {.save}

##도전과제: Games Room 스타일 하고 링크 걸기{.challenge}

__Games Room__의 HTML 과 CSS 를 수정해서 웹페이지가 이렇게 보이게 만드세요: 

![screenshot](rooms-games-challenge.png)

힌트:   `gamesroom.css` 에서 배경색, 폰트 색과 테두리 색을 바꿔야 합니다. 저 밝은 녹색은 `chartreuse`란 이름입니다.  

힌트:  `gamesroom.html`에 `hall.html`로 링크되는  `<a>` 링크를 더해야 합니다. .

## 프로젝트를 저장하세요 {.save}

# 3 단계: 링크를 문처럼 보이게 만듭시다 {.activity}

링크를 텍스트로만 만들 필요는 없습니다.  `<div>`를 사용하여 클릭 할 수 있는 문을 만듭시다.

##단계별 체크리스트 { .check}

+ `index.html`을 열고 __TV Room__ 링크 텍스트 주변에  `<div>` 를 삽입하세요. `<a>` 안쪽에 있어야 클릭 됩니다.

  `id="hall2tv"` 를 더해서 현관에서 TV Room으로 가는 문으로 레이블 해서 문을 스타일 할 수 있게 만듭시다. 

  ![screenshot](rooms-tvroom-div.png)  

+  `style.css` 탭을 클릭하고 맨 밑으로 내려가 다음 CSS 를 더해서 문의 크기와 색을 바꿉시다:

	![screenshot](rooms-door-css1.png)

+ 문을 클릭해서 웹페이지를 확인해봅시다.

+ 이제 3면에 테두리를 더해 좀 더 문처럼 보이게 만듭시다:

	![screenshot](rooms-door-css2.png)

+ 그리고 CSS를 더해 문의 텍스트를 더 보게 좋게 만들고요:

	![screenshot](images/rooms-door-css3.png)

+ 또한 문이 떠있는 걸 보셨을 것입니다. 방 안에 문을 넣어서 문제를 고칩시다.

	![screenshot](rooms-door-position.png)	

+ 문을 눌러서  __TV Room__으로 갈 수 있는지 확인해 봅시다.

## 프로젝트를 저장하세요 {.save}

##도전과제: 문 더 더하기! {.challenge}

프로젝트의 다른 링크들도 같은 방법으로 링크를 문으로 만드세요. 

각 문에는:

+ 문 링크를 `<div>`를 써서 수정하고 `hall2games` 같은 id를 써서 스타일 할수 있게 만드세요.

	예를 들면: 

	`<a href="gamesroom.html"><div id="hall2games">Games Room</div></a>`

+ 문 id의 CSS를 방의 `.css` 파일에 넣으세요. _복사_ _붙여넣기_를 사용해서 시간을 아끼세요. 원하신다면 각 문을 다른 모습으로 만들 수 있습니다.

+ 문 위치를 `bottom:` 과  `left:` 나 `right:`를 써서 지정하세요.

현관의 예시입니다:

![screenshot](rooms-hall-doors.png)

TV Room 은 이렇게 보여야 합니다:

![screenshot](rooms-tvroom-door.png)	


# 4 단계: 배경 이미지 더하기 {.activity}

현관을 배경 이미지로 꾸며봅시다.

## 단계별 체크리스트 { .check}


+  `style.css`를 수정해서 현관에 배경 이미지를 삽입합시다:

	![screenshot](rooms-hall-decorated.png)	

	이미지가 반복되어서 방 전체를 채울 것입니다. 


## 프로젝트를 저장하세요 {.save}

##도전과제: Games Room에 배경을 넣으세요. {.challenge}

games room 을 배경으로 꾸밀 수 있나요?

프로젝트에 포함된  `space-invader.png` 배경 이미지를 쓸 수 있습니다.. 

다음 단계가 필요합니다:

+ Games room의 `.room` CSS 에 `background-image`를 더해야 합니다.

꾸며진 방은 이런 모습입니다:

![screenshot](rooms-games-finished.png)	

## 프로젝트를 저장하세요 {.save}

##도전과제: 나만의 것으로 만드세요! {.challenge}

프로젝트에 더 많은 방을 더하세요. _복사_ _붙여넣기_를 사용해서 바꿀 부분들만 바꾸면 시간을 아낄 수 있다는 걸 잊지 마세요.

각 방에는 다음과 같은 단계가 필요합니다:

+ `.html` 파일 만들기
+ 새 `room'에 문 링크 만들기
+ 새 방과 문에 스타일 가능한 `.css` 파일 더하기

각 방의 `background-color.` 를 바꿀 수 있습니다. 이미지 아이콘을 눌러서 배경 이미지들을 골라보세요:

![screenshot](rooms-images.png)	

## 프로젝트를 저장하세요 {.save}

