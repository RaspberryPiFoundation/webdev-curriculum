---
제목: 잡지
난이도: HTML & CSS 2
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 { .intro}

이 프로젝트에선 HTML 과 CSS 를 사용해서 두 페이지 배치가 된 여러 페이지의 잡지 웹사이트를 만드는 방법을 배울 것입니다. 또한 다름 프로젝트에서 배운 여러가지 HTML & CSS 테크닉을 다시 짚어갈 것입니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/a41e4e1c5c?outputOnly=true&start=result" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="magazine-final.png">
</div>


# 1 단계: 헤딩과 배경

잡지 형식 웹사이트는 자주 페이지에 작은 아이템을 많이 배치합니다. 먼저 잡지의 헤딩과 배경을 만들 것입니다.

## 단계별 체크리스트 { .check}

+ 이 트링켓을 여세요: <a href="http://jumpto.cc/web-magazine" target="_blank">jumpto.cc/web-magazine</a>. 온라인으로 읽고 있다면 아래의 embedded 된 트링켓을 사용하세요.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/cef5e64bc0" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 헤딩을 더합시다.

	더 좋은 잡지 제목을 골라도 됩니다.

	![screenshot](magazine-heading.png)

+ 헤딩에 스타일을 더할 수 있나요?

	이건 예시지만 원하는 스타일을 고르 셔도 됩니다:

	![screenshot](magazine-heading-style.png)

+ 이제 그래디언트를 사용하여 흥미로운 배경을 만들고 잡지에 사용할 폰트를 고릅시다. 

	그래디언트를 만드는 방법을 기억나게 해줄 예시 입니다: 

	![screenshot](magazine-background.png)

## 프로젝트를 저장하세요 {.save}

# 2 단계: 세로 단 만들기

웹사이트에선 자주 다중-세로 단 배치를 사용합니다. 잡지에 사용할 2중 세로 단 배치를 만들어 봅시다. 

## 단계별 체크리스트 { .check}

+ 먼저 두 세로 단  `div`들을 만드세요.

	`index.html`에 강조된 HTML을 더하세요:

	![screenshot](magazine-columns.png)

+ 이제 세로 단 div를 스타일 해서 하나는 왼쪽으로 float하고 하나는 오른쪽으로 float 하게 만듭시다. 

	![screenshot](magazine-columns-style.png)

	각 세로단은 50%이하이니 패딩을 넣을 자리가 있습니다. 

	세로단에 무언가를 더해야 효과가 보일 것입니다. 

+ 두번째 세로 단 위에 고양이 이미지를 더합시다. 

	![screenshot](magazine-kitten.png)

	고양이 이미지가 페이지 반을 좀 건너서 두번째 세로 단 쪽에 위치한걸 봐주세요.

	하지만 조금 너무 큽니다!

+  `max-width: `를 사용하여 이미지들을 포함될 단 안에 맞도록 조정합시다. 

	다음 스타일을  `style.css`에 더하세요.

	![screenshot](magazine-img-width.png)

	이 스타일은 고양이 뿐만이 아니라 잡지에 사용될 모든 이미지에 적용됩니다.

+ 이제 이미지에 `photo` class 를 더하여 스타일 할 수 있도록 만듭시다:

	![screenshot](magazine-photo.png)

+ 이미지에 그림자와 트위스트 스타일을 더해 페이지에서 photo가 튀어나오게 보이도록 만듭시다:

	![screenshot](magazine-photo-style.png)

	결과가 마음에 들때까지 적당히 수정해주세요.


# 3 단계: 잡지의 아이템 스타일 하기

배치를 좀 더 흥미롭게 만들어 봅시다.

## 단계별 체크리스트 { .check}

+ 이미지에 `class`를 써서 `div` 를 두르고 `h2` 헤딩을 더해주세요:

	![screenshot](magazine-item.png)

+ 이제 아이템과 헤딩을 스타일 해주세요.

	이건 예시고 원하시는 대로 수정해주세요:

	![screenshot](magazine-item-style.png)

## 프로젝트를 저장하세요 {.save}

##도전과제: 왼쪽 세로단에 아이템을 더하세요 {.challenge}

왼쪽 세로단에 ordered list 와 gradient 텍스트 스티커를 더할 수 있나요?

예시 입니다:

![screenshot](magazine-challenge1-example.png)

다음은 예시의 코드입니다만 원하시는 대로 수정하시거나 직접 만들어 넣으실 수 있습니다,

HTML:

![screenshot](magazine-challenge1.png)

CSS:

![screenshot](magazine-challenge1-style.png)


## 프로젝트를 저장하세요 {.save}


# 4 단계: 두번째 페이지 더하기

잡지 웹사이트에 다른 페이지를 더해봅시다. 

## 단계별 체크리스트 {.check}

+ 프로젝트에 새 페이지를 더하고  `page2.html` 라고 이름 지으세요:

![screenshot](magazine-page2.png)

+ 2페이지는 첫번째 페이지와 상당히 비슷하니  `index.html` html을 복사해서  `page2.html`에 더해 넣으세요.

![screenshot](magazine-page2-html.png)

두 페이지 다 같은  `style.css` 를 사용하니 스타일을 공유한다는 점에 유의해주세요.

+ 페이지 2의 `<h1>` 제목을 바꾸세요: 

![screenshot](magazine-page2-h1.png)

+ 이제 2 페이지와 첫번째 페이지 사이에서 넘어갈 수 있게 링크를 더해야 합니다.

`index.html`로 돌아가서 두번째 세로단의 div 안쪽에 링크를 넣으세요:

![screenshot](magazine-page2-link.png)

+ 링크를 눌러서 2 페이지로 넘어갈 수 있는지 확인해보세요.

##도전과제: 첫번째 페이지로 돌아갈 링크 더하기 {.challenge}

`page2.html` 에 링크를 더해서 클릭하면 첫번째 페이지로 돌아갈 수 있게 만들 수 있나요?

힌트: 페이지 2로 넘어가게 만들 때 사용했던 HTML을 보세요.


##도전과제: 두번째 페이지를 채워 넣으세요 {.challenge}

다음은 예시에 사용된 코드입니다만 원하시는 대로 'div'를 바꾸거나 직접 만들어도 됩니다.

![screenshot](magazine-page2-challenge.png)

이미지 아이콘을 클릭해서 사용 가능한 이미지를 확인해보세요:

![screenshot](magazine-animation-image.png)

원하는 이미지를 직접 업로드 할 수 있다는 점도 잊지 마세요. 직접 업로드 할 이미지는 미리 허락을 받아야 한다는 걸 기억하세요. 

![screenshot](magazine-upload-images.png)

# 5 단계: 애니메이션 더하기

잡지에 재미있는 애니메이션을 더해봅시다.


## 단계별 체크리스트 {.check}

+ `index.html` 로 가서 `greenrobot.png` 이미지를 페이지 상단에 넣어주세요.

![screenshot](magazine-animation-image.png)

+ 이제 CSS를 넣어서 로봇을 움직이게 만드세요.

![screenshot](magazine-animation-css.png)


##도전과제: 다른 애니메이션 추가하기 {.challenge}

잡지의 2 페이지에 다른 애니메이션을 추가할 수 있나요? 

![screenshot](magazine-animation-challenge.png)


