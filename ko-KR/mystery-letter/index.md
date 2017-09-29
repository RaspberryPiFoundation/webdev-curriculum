---
제목: 수수께끼의 편지
난이도: HTML & CSS 1
언어:  ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 {.intro}

이 프로젝트에선 각 단어가 다른 신문, 잡지, 만화, 또는 다른 소재에서 잘라 만든 것처럼 보이는 수수께끼 편지를 만들 것입니다.

![screenshot](letter-final.png)

# 1 단계: 메시지를 선택하세요 {.activity}

수수께끼의 편지는 영화나 책에서 비밀스러운 메시지를 보내기 위해 사용됩니다. 

## 단계별 체크리스트 { .check}

+ 수수께끼의 메시지의 내용을 생각해 보세요, 12 단어 정도가 적당합니다. 적당한 메시지가 생각 안 난다면 다음 예시를 사용하세요: `다음 단서는 금고 안에 있다. 코드는 65536이다.'

+ 메시지를 따로 적어 놓거나 기억해두세요.

# 2 단계: 메시지 수정하기 {.activity}

메시지를 웹페이지에 올립시다.

## 단계별 체크리스트 { .check}

+ 다음 트링켓을 여세요: <a href="http://jumpto.cc/web-letter" target="_blank">jumpto.cc/web-letter</a>. 혹은 온라인으로 읽고 있다면 아래의 embedded 된 트링켓을 사용하세요.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b5fbcf112e" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+  `<p>` 문단 태그는 `생일 축하` 프로젝트에서 배웠고 `<span>` 태그는 문단안에 짧은 텍스트 조각들을 정리 시켜 넣어서 스타일 하는데 사용합니다

![screenshot](letter-placeholder.png)

## 단계별 체크리스트 { .check}

+ 메시지의 각 단어들을 각자 `<span>`안에 넣어서 바꾸세요. 메시지가 다른 길이라면 `<span>` 태그를 더하거나 지워야 할 것입니다.

![screenshot](letter-message.png)

## 단계별 체크리스트 { .check}

+ run 버튼을 눌러서 트링켓을 확인해보세요t.

	단어들을 보면 페이지에 붙여 놓은 것처럼 보이도록 스타일 된 것을 볼 수 있습니다.

# 3 단계: class 스타일 사용하기{.activity}

## 단계별 체크리스트 { .check}

+  `<span>` tag 안의 `class=""` 를 보셨 나요? 이걸 사용하여 하나 이상의 것들을 같은 방식으로 스타일 할 수 있습니다.

+ `magazine1` 클래스를  `<span>` tags 몇개 안에 넣고 웹페이지를 시험해보세요.

![screenshot](letter-magazine1.png)

## 단계별 체크리스트 { .check}

+ 요소에 하나 이상의 class를 더할 수 있습니다. 단순히 사이에 스페이스를 남겨두세요. `<span>` tag 중 하나에  `big` class 를 넣고 웹페이지를 시험해보세요.. 

![screenshot](letter-big.png)

## 프로젝트를 저장하세요 {.save}

## 도전과제: 메시지 스타일해보기 {.challenge}

주어진 스타일을 사용하여 메시지가 수수께끼의 편지처럼 보이게 만드세요.

다음 class 들을  `<span>` 태그에 더하세요: 

+ `newspaper`, `magazine1`, `magazine2`

+ `medium`, `big`, `reallybig`

+ `rotateleft`, `rotateright`

+ `skewleft`, `skewright`

하나의 `<span>`에 각 줄 에서 한 종류 이상을 넣지 마세요.

편지의 예시 입니다:

![screenshot](letter-challenge1.png)

## 프로젝트를 저장하세요 {.save}

# 4 단계: class 수정하기  {.activity}

## 단계별 체크리스트 { .check}

+  __'style.css'__ 탭을 클릭하고 사용하고 있던 `newspaper` CSS class 에 쓰는 스타일을 찾으세요.

![screenshot](letter-newspaper.png)

+ CSS 파일의 class 이름 앞에는 마침표가 많지만 HTML 문서의 `<span>` tag 에는 없는데 유의해주세요.

+ 이제 수수께끼의 편지를 스타일 할 때 사용했던 다른 CSS class들을 보세요. 다음을 찾을 수 있나요?:

	+ `magazine1` 스타일이 어떻게 텍스트를 전부 대문자로 만드는지.

	+ `magazine2` 스타일이 어떻게 텍스트 뒤에 이미지를 넣는지.

![screenshot](letter-magazines.png)

+ `magazine2`의  `background-image'를 `canvas.png`로 바꾸면 어떻게 되나요? `pink-pattern.png` 이 좋으시다면 다시 바꿔 넣으세요.

또한 잡지 스타일의 색을 바꿀 수도 있습니다.

+ 단어들을 돌리고 삐뚤어지게 만드는 CSS를 찾으세요:

![screenshot](letter-rotate-skew.png)

숫자를 바꿔서 다른 효과를 만들고 페이지를 확인해보세요.

# 5 단계: 새 class 만들기  {.activity}

만화책에서 잘라온 듯한 새로운 스타일을 만듭시다. <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> 에서 무료로 사용할 수 있는 폰트를 많이 제공합니다.. 

## 단계별 체크리스트 { .check}

+ __style.css__ 파일에 `comic` 클래스를 만들어 넣으세요. `magazine2` 뒤쪽이 적절한 자리입니다. class 이름 앞의 마침표를 잊지 마세요. 

![screenshot](letter-comic1.png)

'The Rule is empty' 라는 경고 메시지를 받아도 걱정하지 마세요. 다음에 그 부분을 고칠 것입니다.

+ Comic CSS class 에 CSS 를 더하세요 . 원하신다면 다른 색깔을 사용하여도 좋습니다.  <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>에 사용할 수 있는 색깔이 나열되어 있습니다.

![screenshot](letter-comic2.png)

+ HTML 문서에 있는 `<span>` 태그 일부에 comic style을 사용하고 웹사이트를 확인해보세요.

![screenshot](letter-comic-output.png)

+ 이제 재미있는 폰트를 더해 볼 수 있습니다. 새 브라우저 탭을 열고 <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> 으로 가서 __'bangers'__를 검색해 보세요:

![screenshot](letter-fonts1.png)

+ Quick-use 버튼을 누르세요:

![screenshot](letter-fonts2.png)

+ 새 페이지가 열릴 것 입니다. 다음이 보일때까지 아래로 내리세요:

![screenshot](letter-fonts-link.png)

그리고 강조된 코드를 복사하세요.

+ 방금 구글 폰트에서 복사한 `<link>` 코드를 웹페이지의 `<head>` 에 붙여 넣으세요:

![screenshot](letter-fonts-head.png)

이것으로 웹페이지에서 'bangers' 폰트를 사용할 수 있습니다.

+ 구글 폰트로 돌아가 font-family 코드를 복사하세요:

![screenshot](letter-fonts-bangers.png)

+ 이제 트링켓의 __'style.css'__ 파일로 돌아가 font-family 코드를 comic 스타일에 붙여 넣으세요:

![screenshot](letter-fonts-comic.png)

+ 웹사이트를 다시 확인해보세요. 이런 느낌의 모습이어야 합니다: 

![screenshot](letter-fonts-output.png)

## 프로젝트를 저장하세요 {.save}

## 도전과제: 컴퓨터에서 프린트 한 스타일 {.challenge}

옛날 컴퓨터에서 프린트한 스타일을 만들고 단어 몇개에 적용시켜보세요:

![screenshot](letter-fonts-printout.png)

다음이 필요합니다:

+ <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> 에서 `VT323` font family, 구글 폰트를 사용하는 방법은 5단계를 돌아보세요. 

+ `computer-printout-paper.png` 배경 이미지. 배경 이미지를 사용하는 방법은 4 단계를 돌아보세요.

## 도전과제: 스타일 직접 만들기 {.challenge}

이제 나만의 class 스타일을 만들고 수수께끼 편지를 더욱 더 흥미롭게 만들어보세요. 이전 프로젝트에서 배웠던 CSS를 사용하고  __style.css__ 의 예시를 보고 영감을 얻어보세요. 

예시입니다:

![screenshot](letter-fonts-challenge3.png)

트링켓에서 이미지 탭을 클릭해서 사용가능한 이미지들을 볼 수 있습니다.
다음 포함된 이미지 중 하나를 사용해서 이미지 배경을 설정해보세요:

+ `rough-paper.png`

+ `canvas.png`

트링켓 계정이 있다면 '이야기 전하기' 프로젝트에서 했던 것처럼 이미지를 직접 업로드 할 수도 있습니다.

<a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> 에서 좋아하는 폰트를 찾아서 `<link>` 와CSS code 를 트링켓으로 복사해와서 사용하세요. 

## 프로젝트를 저장하세요 {.save}
