---
제목: 로봇 조립하기
난이도: HTML & CSS 2
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 { .intro}

이 프로젝트에선 이미지의 위치를 지정해 로봇을 만드는 방법을 배울 것입니다.

![screenshot](robot-final.png)

# 1 단계: 로봇 눈 만들기 { .activity}

로봇에 눈을 달아 줘봅시다!

## 단계별 체크리스트 { .check}

+ 온라인으로 하고 있다면 이 트링켓을 열어주세요: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>. 또는 아래의 embedded 된 트링켓을 사용해도 됩니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b29b50e571" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 이 프로젝트의 각 이미지는 각자의 이름(혹은 __id__)가 있습니다. 예를 들자면 얼굴과 눈 이미지의 HTML (코드 8번째 줄에서 시작하는‘face’, ‘eyes1’ 와 ‘eyes2') 은 이렇습니다:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ 이미지의 id에 `#`을 사용하여 각각의 스타일을 줄 수 있습니다. 이걸로 각 이미지를 따로 스타일 할 수 있게 해줍니다.

`style.css` 파일을 클릭하세요. 로봇의 얼굴과 다른 이미지가 다른 크기 인걸 보셨 나요?

![screenshot](robot-id.png)

+ 이 CSS 코드를 넣어서 로봇의 눈을 스타일 하세요:

```
#eyes1 {
    width: 200px;
}
```

CSS에선 `#eyes1`만 사용해서 `eyes1` 이미지만 스타일 하고있다는데 주의하세요. 원하신다면 `#eyes2` 나 `#eyes3` 를 쓸 수도 있습니다!

![screenshot](robot-eyes-width.png)

+ 각 이미지가 다음 이미지에 이어서 나오고 있다는 걸 보셨 나요? 이것은 __relative__ positioning이라고 불립니다. 브라우저가 정확히 어디에 로봇의 눈을 둘지 지정하고 싶다면 __absolute__ positioning 을 사용해야 합니다.

`eyes1` 이미지를 위해 다음 3줄의 코드를 CSS에 더해주세요:

```
position: absolute;
top: 200px;
left: 100px;
```

로봇의 눈이 제대로 된 위치로 옮겨 간 것을 볼 수 있습니다.

![screenshot](robot-eyes-position.png)

이 CSS는 브라우저에게 웹페이지의 상단/왼쪽에서 얼마나 멀리 이미지를 표기할지 알려줍니다.

![screenshot](robot-eyes-position2.png)

또한 `bottom` 을 `top` 대신 써서 바닥에서부터 얼마나 멀리서 이미지를 보여주게 하거나 `right` 을 `left` 대신 사용할 수도 있습니다.

# 2 단계: 로봇에게 입을 달자 { .activity}

로봇에게 입을 달아주죠!

## 단계별 체크리스트{ .check}

+ 다음 CSS코드를 넣어 `mouth1` 이미지를 스타일 합시다:

```
#mouth1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ 로봇의 입이 꽤 작아 보이고 제대로 위치하고 있지 않군요.

![screenshot](robot-mouth.png)

CSS를 고쳐서 이 문제를 해결할 수 있나요?

## 프로젝트를 저장하세요 {.save}

##도전과제: 나만의 로봇을 디자인해보세요 {.challenge}
지금까지 배운 기술을 써서 로봇을 만드는 걸 완성시키세요. 완성된 로봇의 예들입니다:

![screenshot](robot-examples.png)

## 프로젝트를 저장하세요 {.save}

##도전과제: 이미지 직접 더하기 {.challenge}
로봇에 사용할 추가 이미지들을 찾아서 로봇에 웹페이지에 넣을 수 있나요? 심지어 로봇의 얼굴을 자기 얼굴로 바꿔 넣을 수도 있습니다!

```
<img id="face" src="myFace.png">
```

## 프로젝트를 저장하세요 {.save} 
