---
제목: 이야기 해주세요
난이도: HTML & CSS 1
언어: ko-KR
embeds: "*.png" 
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 { .intro}

이 프로젝트에선 웹페이지를 만들어 이야기나 농담, 시를 전할 것입니다.

![screenshot](story-final.png)

# 1 단계: 줄거리를 정해주세요 { .activity}

코딩 하기 전에 먼저 전해줄 이야기를 정해야 합니다.

## 단계별 체크리스트 { .check}

+ 전하고 싶은 이야기에 대해서 생각해보세요. 다음 중 하나일 수 있습니다:
	+ 유명한 이야기;
	+ 직접 만든 이야기;
	+ 당신이나 알고있던 사람이 겪었던 이야기.

	혹은 이야기일 필요도 없이 농담이나 시 혹은 원하는 무엇이던 괜찮습니다!

# 2 단계: 이야기 수정하기 { .activity}

이야기를 담을 웹페이지의 HTML 콘텐츠와 CSS 스타일을 수정하는 것으로 시작합시다.

## 단계별 체크리스트 { .check}

+ 이 트링켓을 여세요t: <a href="http://jumpto.cc/web-story" target="_blank">jumpto.cc/web-story</a>. 혹은 온라인으로 읽고 있다면 아래의 embed 된 트링켓을 사용하세요.

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/8083cfebb3" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

+  'Happy Birthday' 프로젝트에서 배웠듯이 웹페이지의 내용은 HTML 문서의 `<body>` 안으로 들어갑니다.

	코드의 7번째 줄로 가면 e`<body>` 와 `</body>` 태그 안에 들어있는 웹페이지 콘텐츠가 보일 것입니다.

	![screenshot](story-html.png)

+ 웹페이지의 부분들을 만들기 위해 어떤 태그가 사용되고 있는지 알 수 있겠 나요?

	![screenshot](story-elements.png)

	+ `<h1>` 란 __헤딩__입니다. 1에서 6 사이의 숫자를 사용해 다른 크기의 헤딩을 만듭니다;
	+ `<div>` 란 __division__의 줄임 말이며 몇가지를 뭉쳐 구분하는데 사용됩니다. 이 웹페이지에선 div를 사용해 이야기의 부분들을 뭉쳐 구분할 것입니다;
	+ `<img>` 란  __이미지__입니다;
	+ `<p>` 는 텍스트 __문단__ 입니다.

##도전과제: 수정해보세요 {.challenge}
HTML 과 CSS 코드를 수정해 웹페이지를 수정해보세요.

![screenshot](story-changes.png)

웹페이지에 사용되는 색을 바꾸거나 다음의 폰트들을 사용해볼 수 있습니다 <span style="font-family: Arial;">Arial</span>, <span style="font-family: Comic Sans MS;">Comic Sans MS</span>, <span style="font-family: Impact;">Impact</span> and <span style="font-family: Tahoma;">Tahoma</span>.

도움이 필요하다면 'Happy Birthday' 프로젝트를 참조하세요.

## 프로젝트를 저장하세요 {.save}

# 3 단계: 이야기 전하기 { .activity}

이야기의 두번째 부분을 더해봅시다.

## 단계별 체크리스트 { .check}

+ 코드의 17번쨰 라인으로 간 후 `<div>` 와 `</div>` 태그를 한 개씩 더해주세요. 이것으로 이야기의 다음부분을 전할 새 박스가 만들어 질것입니다. 

	![screenshot](story-div.png)

+  `<div>` 태그 안에 문단을 더하세요.

	![screenshot](story-paragraph.png)

+ 마지막으로 이 박스에 다음 코드를  `<div>` 태그 안에 더해서 이미지를 더할 수 있습니다:

	```
	<img src="">
	```

	`<img>` 태그는 다른 태그와는 다르게 마침 태그가 없다는데 유의해주세요.

+ HTML 이미지는 이미지의 __source__ 를 speech marks안에 더해야 합니다. 이야기에 넣을 이미지를 찾아봅시다.

	<a href="http://jumpto.cc/web-images" target="_blank">jumpto.cc/web-images</a>로 간 후 이야기에 더하고 싶은 이미지를 찾아보세요.

+ 이미지를 오른쪽 클릭 하고 'Copy image URL'을 클릭하세요. URL이란 이미지의 주소입니다.

	![screenshot](story-url.png)

+ URL을 `<img>` tag 안의 speech marks 에 붙여 넣으세요. 이미지가 나타날 것입니다!

	![screenshot](story-image.png)

+ __트링켓 계정이 있다면__ 웹페이지에 직접 이미지를 업로드 할 수 있습니다! 트링켓 상단의 이미지 아이콘을 클릭하고  'upload'를 클릭하세요.

	![screenshot](story-upload.png)

+ 컴퓨터에서 원하는 이미지를 찾아서 트링켓으로 드래그 해 넣으세요.

	![screenshot](story-drag.png)

+ 그리고 다음과 같이 이미지의 이름을  `<img>` 태그의 speech marks 사이에 넣으면 됩니다:

	```
	<img src="buildings.png">
	```

## 프로젝트를 저장하세요 {.save}

##도전과제: 계속 하세요! {.challenge}
이 프로젝트에서 배운 것을 사용해 이야기를 끝마치세요! 다음은 예시입니다:

![screenshot](story-final.png)

## 프로젝트를 저장하세요 {.save}
