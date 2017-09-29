---
제목: 스티커!
난이도: HTML & CSS 2
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 {.intro}
 
이 프로젝트에선 웹페이지를 꾸미는데 사용할 여러가지 재미있는 스티커를 만들 것입니다. 또한 스티커에 그라데이션을 더해 멋지게 만드는 방법도 배울 것입니다.

![screenshot](stickers-finished.png)

# 1 단계: 선형 그라데이션 스티커 만들기 {.activity}

그라데이션이란 한 색에서 다른 색으로 서서히 변해가는 것을 말합니다. 그라데이션을 이용하면 멋진 효과를 만들 수 있습니다. 여기 선 그라데이션을 사용해 웹페이지에 사용할 스티커를 만들어 볼 것입니다. 

+ 다음 트링켓을 여세요: <a href="http://jumpto.cc/web-stickers" target="_blank">jumpto.cc/web-stickers</a>. 혹은 온라인으로 읽고 있다면 아래의 embed 된 트링켓을 사용하세요. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/af0ea6fa35" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 'I <3 Coding' 스티커를 만들어 봅시다. 

	`sticker` 클래스 와  `coding` id에 `<div>` 를 사용해여 스타일 가능하게 만듭시다: 

	![screenshot](stickers-coding-error.png)


+ 에러가 생기는 걸 보셨 나요? 이건 '<' 이 HTML에선 특수문자이기 때문입니다. '<' 대신에 특수 코드 `&lt;`를 사용해보세요. 

	코드 `&lt;`을 사용하도록 만들어서 에러를 없애세요. 

	![screenshot](stickers-coding-fixed.png)

	`<br>` 은 새 줄을 만듭니다. 

+ 이제 스티커를 더 흥미로워 보이게 만듭시다. 

	`style.css` 파일로 가세요. `.sticker` 클래스를 사용할 수 있는 걸 볼 수 있습니다. 이것으로 스티커를 페이지에 배치하고 중심을 잡게 만들 것입니다.

	스티커에 `coding`이란 id를 더했다는 걸 기억하세요. `style.css`의 제일 밑에 다음 코드를 넣어서 텍스트를 스타일 하세요:

	![screenshot](stickers-coding-font.png)

+ 이제 스티커의 배경에 그라데이션을 넣을 수 있습니다. 선형 그라데이션은 한색에서 다른 색으로 직선을 따라 바뀝니다.

	이 그라데이션은 위는 빨간색에서 아래쪽은 마젠타 색으로 바뀔 것입니다. 다음 그라데이션 코드를 `coding` 스타일에 더하세요:

	![screenshot](stickers-coding-gradient.png)

+ 패딩과 둥근 모서리를 더해 결과물을 개선할 수 있습니다.

	다음 강조된 부분의 코드를 넣으세요:

	![screenshot](stickers-coding-padding.png)

	`padding` 스타일은 위쪽 과 아래쪽에 50px, 그리고 오른쪽 왼쪽으론 30px의 패딩을 더합니다.


## 프로젝트를 저장하세요 {.save}

# 2 단계: 원형 그라데이션 스티커 만들기 {.activity}

또한 중심에서 바깥쪽으로 나가며 색이 바뀌는 그라데이션도 있습니다. 이것은 원형 그라데이션이라고 불립니다. 

+ `HTML & CSS.`이라는 텍스트로 스티커를 만듭시다.  `&` 은 HTML에서 다른 엔코딩이 필요한 또다른 글자입니다. `&amp;`로 바꿔주세요.

	다음 강조된 코드를 더해 새 스티커를 만드세요: 

	![screenshot](stickers-web-html.png)

+ 이제 `style.css` 파일로 간 후 새 스티커에 스타일을 더해주세요:

	![screenshot](stickers-web-font.png)

	`text-shadow` 코드는 텍스트 오른쪽과 아래쪽으로 2px씩 그림자를 더해 부각되 보이게 만들어 줍니다.

+ 이제 그라데이션을 만듭시다. 이번엔 원형 그라데이션으로요. 색깔은 중심은 노란색에서 시작해서 주황색을 거쳐 빨간색으로 가게 만듭시다.

	![screenshot](stickers-web-gradient.png)

	그라데이션엔 두 색만이 아닌 여러 색을 사용할 수 있다는데 유의해주세요.

+ 패딩과 둥근 모서리를 더해주면 훨씬 나아 보일 것입니다.

	다음 강조된 코드를 더해주세요:

	![screenshot](stickers-web-padding.png)


## 프로젝트를 저장하세요 {.save}

##도전과제: 나만의 그라데이션 스티커 만들기 {.challenge}

이제 나만의 그라데이션 스티커를 만들어 보세요. 선형과 원형 그라데이션을 여러가지 HTML 색을 사용해 만들어보세요. 

다음 단계가 필요합니다:

+ 스티커에 텍스트에 `<div>` 를 `index.html`로 더하고 `sticker` 클래스와 새로운 `id` 주기.
+ `id`에 `style.css`에서 정한 스타일 더해주기. 지금까지 만든 스티커 스타일을 복사해서 붙여 놓고 수정해도 됩니다.

여기에 사용할 수 있는 색깔 이름들이 있으며: [jumpto.cc/web-colours](http://jumpto.cc/web-colours) `tomato`, `firebrick` 이나 `peachpuff`같은 색깔들이 포함되어 있습니다.

텍스트 색을 바꾸려면 `color:`를 사용하세요.

다수의 색을 선형 그라데이션에 사용한 예시입니다:

![screenshot](stickers-save-robots.png)

## 프로젝트를 저장하세요 {.save}

# 3 단계: 이미지로 그라데이션 스티커 만들기  {.activity}

이미지를 사용해서 그라데이션 스티커를 만들 수도 있습니다. 투명한 배경을 가진 이미지를 사용하면 그라데이션이 뒤쪽으로 보일 것입니다.

+ 먼저 이미지를 사용한 스티커를 만듭시다 

	프로젝트엔 이미 `purplerobot.png`란 이미지가 있습니다.

	다음 강조된 코드를 `index.html`에 더하세요:

	![screenshot](stickers-purple-html.png)

	`height`를 조정해서 이미지 크기를 조절할 수 있습니다. width는 자동으로 바뀔 것입니다.

+ 이제 스타일 코드를 더해 이미지 스티커에 그라데이션 배경을 만들어 줍시다:

	![screenshot](stickers-purple-css.png)


## 프로젝트를 저장하세요 {.save}

##도전과제: 나만의 이미지 스티커를 만들어 보세요 {.challenge}

이제 직접 그라데이션을 사용한 이미지 스티커를 만들어보세요

다음과 같은 과정이 필요합니다:

+ 이미지가 포함된 새 스티커 `<div>` 를 `index.html`에 더하기. 
+ sticker div에 `sticker` 클래스와 새 id 주기.
+ id에 그라데이션과 패딩이 있는 스타일 만들어 주기. 

이 프로젝트엔 여러가지 로봇 이미지가 이미 들어있습니다. 이미지 아이콘을 클릭해서 사용 가능한 이미지들을 확인해보세요. 

![screenshot](stickers-images.png)

선형 그라데이션을 사용한 이미지 스티커의 예시입니다:

![screenshot](stickers-blue-robot.png)


## 프로젝트를 저장하세요{.save}

# 4 단계: 수평 그라데이션 {.activity}

그라데이션은 수평이나 수직일 수도 있습니다.

+ 이미지 스티커를 하나 더 만듭시다.

	이번엔 `greenrobot.png`를 씁니다. 다음 코드를 `index.html`로 더하세요:

	![screenshot](stickers-green-html.png)

+ 보통 선형 그라데이션은 위에서 아래로 가지만 `to right`를 더하면 왼쪽에서 오른쪽으로 가게 만들 수 있습니다.

	강조된 부분의 코드를 `style.css`로 더해서 로봇 스티커에 수평 그라데이션을 더하세요.

	![screenshot](stickers-green-style.png)

	그라데이션이 왼쪽에선 초록색으로 시작해 오른쪽으로 노란색이 되갑니다.

+ 로봇이 무언가 말하고 싶어하는 거 같지 않나요? 스티커에 텍스트를 더해봅시다. 

	`index.html`간 후 'Hello!'란 텍스트를 로봇 스티커에 더하세요. `<span>`안쪽에 넣고 id를 줘서 스타일 가능하게 만드세요:  

	![screenshot](stickers-green-span.png)

+ 텍스트를 더 크게 만들고 자리를 잡아주면 더 낫게 보일 것입니다.

	텍스트 위치를 정해주려면 `position: relative;` 를 `#greensticker`에 더해주고 `position: absolute` 를 `#greentext`에 더해야 합니다. 이 부분은 `로봇 만들기`프로젝트에서 더 자세히 설명 되어 있습니다. 

	다음 강조된 코드를 `style.css`에 더해주세요:

	![screenshot](stickers-green-text-style.png)

	이제 'Hello!' 텍스트는 스티커의 오른쪽 아래 구석에 비례해서 위치합니다. 

## 프로젝트를 저장하세요 {.save}

# 5 단계: 대각 그라데이션  {.activity}

또한 모서리에서 모서리로 가는 대각형 그라데이션을 만들 수도 있습니다.

+ `firerobot.png` 이미지를 사용한 스티커를 `index.html`에 더하세요:

	![screenshot](stickers-fire-html.png)

+ 대각 그라데이션을 줄 땐 두 방향을 사용합니다. 예시엔 `왼쪽 하단으로`를 사용합니다.

	이 스타일을 `style.css`에 더해서 이 새 로봇 스티커에 대각 그라데이션과 멋진 border를 주게 만듭시다:

	![screenshot](stickers-fire-gradient.png)

	`outline`을 사용하면 border 밖에 새 border를 만들 수 있다는 점에 주의해주세요.
	`outline-offset`은 border와 outline 사이에 공간을 만들어줍니다.

+ 스티커에 텍스트를 더해봅시다. 

	"ROBOTS!"란 텍스트를 가진 `<span>`을 `index.html`로 더하기 id를 줍시다. 

	![screenshot](stickers-fire-span.png)

+ 이제 다음 스타일을 더해 텍스트의 위치를 정할 수 있습니다:

	![screenshot](stickers-fire-text-style.png)

+ 마지막으로  `transform: rotate`를 사용해 텍스트를 비틀어보죠.

	![screenshot](stickers-fire-rotate.png)

	텍스트가 돌아간 각도를 조정해 보세요!


## 프로젝트를 저장하세요 {.save}

##도전과제: 스티커 더 만들기 {.challenge}

이제 다른 그라데이션 방향, 이미지와 텍스트와 border, outline을 이용해 여러가지 스티커를 만들어봅시다.

만들었던 스티커에 수정을 가해 새로운 스티커를 만들어도 됩니다.

대각선 그라데이션을 사용한 예시입니다:

![screenshot](stickers-dog-robot.png)

## 프로젝트를 저장하세요 {.save}
