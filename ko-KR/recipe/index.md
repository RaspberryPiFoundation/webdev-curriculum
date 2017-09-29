---
제목: 레시피
난이도: HTML & CSS 1
언어: ko-KR 
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...
 
# 소개 { .intro}

이 프로젝트에선 제일 좋아하는 레시피를 올릴 웹사이트를 만드는 방법을 배울 것입니다.

![screenshot](recipe-final.png)

# 1 단계: 레시피 선택하기 { .activity}

코딩을 시작하기 전에 레시피를 선택해야 할 것입니다.

## 단계별 체크리스트 { .check}

+ 친구들과 공유하고 싶은 레시피를 선택하세요. 레시피는:
	+ 온라인에서 찾은 것;
	+ 가장 좋아하는 음식;
	+ 직접 지어낸 레시피!

이 프로젝트에서 사용되는 예시용 레시피는 바나나 밀크셰이크 입니다. 직접 레시피를 찾을 수 없다면 이 레시피를 사용하세요.

# 2 단계: 재료 { .activity}

레시피에 필요한 재료들은 나열해봅시다.

## 단계별 체크리스트 { .check}

+ 다음 템플릿 트링켓을 열어보세요: [jumpto.cc/trinket-template](http://jumpto.cc/trinket-template). 온라인으로 읽고 있다면 아래의 embed 된 트링켓을 사용해도 됩니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ef4c882ae6" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 재료를 나열 하는 데는 `<ul>` tag를 사용한 __unordered list__를 사용할 것입니다. 템플릿의 8번 줄로 간 후 이 HTML을 더하면서 `<h1>`의 제목을 자신의 레시피의 제목으로 바꿔 넣으세요.

```
<h1>Banana Milkshake</h1>

<h3>Ingredients:</h3>

<ul>

</ul>
```

+ 웹사이트를 보면 두개의 헤딩이 보여야 할 것입니다.

![screenshot](recipe-headings.png)

하지만 아직 재료를 하나도 더하지 않았으니 나열 된 건 보이지 않을 것입니다!

+ 다음 작업은 리스트에 넣을 항목들을 `<li>` tag를 사용해서 넣는 것입니다. 다음 코드를 `<ul>` 태그 안에 넣으세요:

```
<li>1 banana</li>
```
![screenshot](recipe-ul.png)

리스트가 정렬되지 않았기 때문에 리스트의 항목들에 번호가 없고 대신 점이 찍혀 있을 것입니다.

##도전과제: 더 많은 재료{.challenge}
당신의 레시피에 사용될 모든 재료들을 더할 수 있겠 나요?

웹페이지는 이렇게 되야 할 것입니다:

![screenshot](recipe-more-ingredients.png)

## 프로젝트를 저장하세요 {.save}

# 3단계: 방법 { .activity }

다음으로 어떻게 이 레시피를 만들 것인지를 설명합시다.

## 단계별 체크리스트 { .check}

+ 방법을 쓰기 위해 다른 리스트를 만들 것이지만 이번엔 '<ol>` 태그를 사용한 __ordered list__를 쓸 것입니다.

ordered list 는 번호로 정렬된 리스트이며 각 단계의 순서가 중요할 때 사용합니다.

이 코드를 재료 리스트 아래에 더하세요. 꼭 `<body>` 태그 안엔 남아있도록 만드세요:

```
<h3>Method:</h3>

<ol>

</ol>
```

![screenshot](recipe-method.png)

+ 이제 항목들을 새 정렬된 리스트에 더하기만 하면 됩니다:

```
<li>Peel the banana and add to a blender</li>
```

![screenshot](recipe-ol.png)

항목들이 자동으로 순서가 정해지는 걸 보세요!

##도전과제: 더 많은 단계 {.challenge}
레시피를 만드는데 사용될 모든 단계를 더할 수 있겠 나요?

완성된 방법은 이렇게 생겼을 것입니다:

![screenshot](recipe-more-method.png)

## 프로젝트를 저장하세요. {.save}

# 4단계: 색깔! { .activity}

레시피 웹페이지에 넣을 색깔을 더합시다.

## 단계별 체크리스트{ .check}

+ 웹페이지의 텍스트에 어떻게 색깔 텍스트를 더하는지는 이미 배웠습니다. 이 코드를 `style.css` 파일에 더해 웹사이트의 모든 텍스트를 파란색으로 만듭시다.:

```
body {
    color: blue;
}
```

![screenshot](recipe-blue.png)

+ 브라우저가 `blue`, `yellow` 나 심지어 `lightgreen`이란 색깔도 아는 건 아셨겠지만 사실 500가지 이상의 색깔의 이름을 알고 있다는 건 아셨 나요?

사용할 수 있는 모든 색깔의 리스트가 있습니다: [jumpto.cc/web-colours](http://jumpto.cc/web-colours), 여기엔 `tomato`, `firebrick` 이나 `peachpuff`같은 이름도 있습니다.

텍스트 색깔을 `blue` 에서 `tomato`로 바꿔보세요.

![screenshot](recipe-tomato.png)

+ 또한 브라우저는 140개의 색의 이름을 알고있지만 1600만개 이상의 색깔의 값도 알고 있습니다!


알고 있을 수도 있겠지만 모든 색은 원색들을 조합함으로써 만들 수 있습니다. 브라우저가 어느 색을 보일지 정해 주려면 각 원색을 얼마나 쓸지를 알려주기만 하면 됩니다.

이 원색들의 값은 `0` 에서 `255`사이의 값으로 적힙니다.

![screenshot](recipe-rgb-img.png)

이 코드를 웹페이지의 body에 더해서 연한 노란색의 배경이 보이게 만들어주세요:

```
background: rgb(250,250,210);
```

![screenshot](recipe-rgb.png)

+ 원하신다면 브라우저에서 보일 색을 정하는데 16진수 (혹은 __hex code__)를 사용해도 됩니다. 이 값은 위의 `rgb()` 코드와 비슷하게 작동하지만 hex code 는 언제나 `#`으로 시작하고 16진수의 `00` 과 `ff` 사이의 숫자를 사용해서 빨강, 파랑, 녹색의 값을 정합니다.

![screenshot](recipe-hex-img.png)

CSS의 `rgb()` 코드를 이 16진수로 바꿔 넣으세요:

```
background: #fafad2;
```

![screenshot](recipe-hex.png)

이전과 같은 옅은 노란색이 그대로 보일 것입니다!

## 프로젝트를 저장하세요 {.save}

# 5 단계: 마무리하기 { .activity}

HTML과 CSS를 조금 더 넣어서 웹페이지를 개선해봅시다.

## 단계별 체크리스트 { .check}

+ 레시피의 끝에 <hr> 태그를 사용해 레시피 끝에 수평선을 넣을 수 있습니다.

![screenshot](recipe-hr.png)

이 태그는 `<img>` 태그처럼 끝 태그가 없다는 점에 유의해주세요.

+ 지금 더한 줄은 웹페이지의 다른 부분과 맞지 않는 스타일입니다. CSS 코드를 좀 더해서 고쳐보죠:

```
hr {
    height: 2px;
    border: none;
    background-color: tomato;
}
```

![screenshot](recipe-hr-css.png)

+ 이 CSS 코드를 쓰면 불릿 포인트의 모습도 바꿀 수 있습니다:

```
ul {
    list-style-type: square;
}
```

![screenshot](recipe-ul-css.png)

##도전과제: 더 많은 색깔! {.challenge}
색깔을 색깔 이름, `rgb()` 값과 16진수를 사용해서 바꿔보세요. 사용 할 수 있는 색깔들을 여기서 볼 수 있습니다 <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>.

몇가지 예시 색입니다:

+ 붉은색은 이렇게 쓸 수 있습니다:
	+ `red` (당연하게도!)
	+ `rgb(255,0,0)` (붉은색 최대값에 초록색과 파란색이 없음)
	+ `#ff0000`

+ 올리브색은 이렇게 쓸 수 있습니다:
	+ `olive`
	+ `rgb(128, 128, 0)` (붉은색과 초록색이 섞이고 파란색 없음)
	+ `#808000`

사용하는 색깔이 레시피에 어울리게 만들어 보세요!

## 프로젝트를 저장하세요 {.save}

##도전과제: 리뷰 {.challenge}
친구들에게 레시피의 리뷰를 남겨 달라고 해보세요. 그러려면 다른 리스트를 만들어야 합니다.

![screenshot](recipe-reviews.png)

## Save Your Project {.save}

##도전과제: 더 스타일 하기 {.challenge}
웹페이지에 이미지를 더할 수 있겠 나요? 혹은 폰트를 바꿀 수 있나요? 웹페이지는 이렇게 보여야 합니다:

![screenshot](recipe-final.png)

도움이 될 만한 코드들입니다:

```
font-family: Arial / Comic Sans MS / Courier / Impact / Tahoma;
font-size: 12pt;
font-weight: bold;

<img src="image-link-goes-here">
```

## 프로젝트를 저장하세요 {.save}
