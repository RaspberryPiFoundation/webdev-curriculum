---
제목: 픽셀 아트
난이도: HTML & CSS 2
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 {.intro}

이 프로젝트에선 픽셀 아트 편집기를 만들 것이고 HTML과 CSS를 사용하는것과 더불어 자바스크립트를 사용하여 프로젝트에 상호작용을 넣는 방법을 배울 것입니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/0e102a306b?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="pixel-art-final.png">
</div>

__편집기 사용하는 방법__: 팔레트에서 색깔을 클릭하여 펜 색을 선택하고 픽셀들을 클릭해서 색을 바꾸세요.

# 1단계: 픽셀 격자 만들기 {.activity}

픽셀 그림을 그리는데 사용될 픽셀 격자를 만들어  봅시다. CSS에선 격자와 테이블 배치를 위한 테이블 스타일이 제공됩니다.

테이블엔 칸들이 포함되는 행들이 있습니다. 검은색 배경의 테이블을 만들고 흰색 픽셀을 집어넣죠.

## 단계별 체크리스트 { .check}

+ 다음 트링켓을 여세요: <a href="http://jumpto.cc/web-pixel" target="_blank">jumpto.cc/web-pixel</a>.만약 온라인에서 읽고 있다면 아래의 embedded 된 트링켓을 사용하세요.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/705f264f59" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 다음 html을 'index.html'파일의  `<body>` 로 넣어서 픽셀미술의 컨테이너로 사용될 `<div>` 를 만들고  `art` id를 줘서 스타일 할 수 있게 만드세요.

	![screenshot](pixel-art-art.png)

 	이제 `style.css` 파일로 가서  art `<div>`의 테이블 스타일링을 넣으세요. 픽셀 줄 셋이 모두 같다는데 유의하세요. 첫번째를 타자 쳐 넣고 나머지는 복사하고 붙여 넣어 만드세요. 

	![screenshot](pixel-art-style.png)

	이걸로 경계선이 있는 테이블이 만들어지고 격자 안의 크기를 정합니다.

	아직 별로 재미있어 보이지 않습니다. 픽셀 행을 안에 넣어야 합니다.

 + 이제  `index.html` 파일로 돌아가서 art `<div>` 안에 3행의 픽셀을 더하세요: 

	![screenshot](pixel-art-row.png)

 	이번엔 여러 개가 있기 때문에 class를 사용하여 div들을 스타일 합니다.

 	다음 스타일을 행과 칸에 넣어주세요:

	![screenshot](pixel-art-row-style.png)

 	이제 픽셀들은 검은색 줄 테두리가 있는 격자 안으로 정리될 것입니다.

 + 이제 픽셀 두 행을 더하여 3x3 격자를 만드세요. 복사 붙여넣기로 시간을 아끼는 걸 잊지 마세요.

	![screenshot](pixel-art-grid-3.png)
	
    
##도전과제: 격자 크기 재설정하기 {.challenge}

3x3 은 픽셀그림을 그리기엔 꽤나 작은 크기입니다. 더 크게 만들 수 있나요? 8x8이 픽셀 그림을 그리는데 적당한 크기입니다. 

전부 타자 쳐 넣는 것보다 복사 붙여넣기를 활용해보세요.

![screenshot](pixel-art-grid-8.png)

## 프로젝트를 저장하세요 {.save}

# 2 단계: 픽셀을 색칠하세요 {.activity}

HTML 콘텐츠를 정리하고 CSS 는 스타일 하는데 사용됩니다. 자바스크립트는 웹페이지에 상호작용을 넣어주는 프로그램 언어입니다. 

HTML & CSS를 사용하여 각 배경 픽셀의 색깔을 정해줄 수 있지만 그건 느린 방법입니다! 대신 자바스크립트 코드를 사용하여 클릭하면 픽셀을 자동으로 색칠하게 만들 것입니다.

+ 자바스크립트에선 코드를 돌리려고 할 때 부를 `function(함수)' 안에 넣습니다.

	 `setPixelColour`라는 함수를 만들 것입니다.

	`setPixelColour` 함수 어느 픽셀의 색을 바꿀지 알아야 합니다. 이것이 'input'입니다. 

	다음 코드를 `script.js` 파일에 더해 픽셀의 배경색을 정하게 만드세요:

	![screenshot](pixel-art-set-pixel-colour.png)

	`backgroundColor`은 색깔의 미국식 철자를 사용하는데 주의하세요.

+ 이제 픽셀을 클릭하면 그 함수를 불러와야 합니다.

	HTML 은 `onclick`을 사용해서 요소를 클릭했을 때 함수를 불러옵니다. 'this'를 input으로 지정해서 함수가 어느 픽셀의 색을 바꿀지 알 수 있게 만드세요.

	`index.html`으로 간 후 다음 코드를 첫번째 픽셀에 더해주세요:

	![screenshot](pixel-art-onclick.png)

+ 첫번째 코드를 클릭해서 코드를 시험해보세요. 검은색이 되야 합니다.

	![screenshot](pixel-art-black.png)

	지금은 'onclick` 코드를 첫번째 픽셀에만 더했으므로 다른 픽셀 들에는 적용되지 않았습니다.


##도전과제: 모든 픽셀들 클릭 가능하게 만들기.challenge}

모든 픽셀들이 클릭 가능하게 만들 수 있나요? 복사 붙여넣기로 더 빠르게 작업하세요.

픽셀그림을 빠르게 그려보세요.

![screenshot](pixel-art-black-example.png)

팁:  __Autorun__ 을 클릭해서 모든 픽셀들을 지울 수 있습니다.

# 3 단계: 색깔 팔레트 추가하기 {.activity}

실수하면 픽셀 색을 다시 흰색으로 못 돌리는게 짜증나지 않으셨 나요? 색 팔레트를 만들어서 색을 클릭하면 펜 색을 바꾸게 만들어 그 문제를 고쳐봅시다. 

+ 먼저 펜 스타일을 만드세요. 

	r `style.css` 파일 맨 아래에 다음 코드를 넣으세요:

	![screenshot](pixel-art-pen.png)

+ 이제 그 스타일을 사용할 검은색과 흰색 펜을 만드세요.

	다음 코드를 `index.html` 에서 `<body>`뒤에 넣으세요:

	![screenshot](pixel-art-palette.png)

	`style=` HTML 안에 CSS 넣게 해줍니다, 여기 선 유용하죠. 

+ 팔레트에서 펜 색을 클릭하면 펜의 색이 바뀌게 만들어야 됩니다.

	변수는 정보를 저장하기 위해 사용됩니다. 'script.js'에 펜 색깔 변수를 만들어보죠.

	다음코드를 파일 맨 위에 넣으세요.

	![screenshot](pixel-art-pencolour.png)

	그리고 펜 색깔을 바꿀 함수를 더하세요:

	![screenshot](pixel-art-set-pen.png)

+ 또한 픽셀의 색을 바꿀 때 펜 색깔도 필요할 것입니다.

	`setPixelColour` 함수 을 'black' 대신 `penColour` 변수를 사용하게 만드세요:

	 ![screenshot](pixel-art-use-pen.png)

+ 이제 펜 색을 눌렀을 때 `setPenColour` 함수를 불러오게 해야 합니다.

	강조된 `onclick` 코드를 펜 색에 더하세요:

	![screenshot](pixel-art-palette-onclick.png)

+ 이제 픽셀에 색을 넣었다 지울 수 있는지 펜 색을 바꿔가면서 확인해보세요.


## 프로젝트를 저장하세요 {.save}

##도전과제: 팔레트에 색 더 더하기. {.challenge}

팔레트에 색을 더 더할 수 있나요? 픽셀그림을 그리고 싶은 색을 정해서 넣어보세요.

그리고 멋진 픽셀 그림을 그리세요.

힌트: 밝은 초록색은  `chartreuse`란 이름입니다.

![screenshot](pixel-art-final.png)

클럽 리더에게 Windows Snipping Tool이나 다른 방법으로 오늘 그린 픽셀 그림을 저장할 수 있는지 물어보세요.

## Save Your Project {.save}

