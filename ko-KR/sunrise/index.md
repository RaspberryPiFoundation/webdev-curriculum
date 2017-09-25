---
제목: 일출
난이도: HTML & CSS 2 
언어: ko-KR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# 소개 { .intro}

이 프로젝트에선 CSS를 사용하여 움직이는 일출 애니메이션을 만드는 방법을 배울 것입니다.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="sunrise-final.png">
</div>

# 1 단계: 태양 만들기 { .activity}

먼저 태양 이미지를 더하고 CSS로 위치를 지정합시다.

## 단계별 체크리스트 { .check}

+ 이 트링켓을 여세요 t: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. 혹은 온라인으로 읽고 있다면 아래의 embed 된 트링켓을 사용하세요.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/5085f92143" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ `index.html` 파일의 'body' 안쪽을 보면 하늘과 바다의 'div' 속성들을 찾을 수 있습니다.

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```

+ 태양으로 사용할 이미지는 프로젝트에 이미 들어있습니다. 

    태양 'div'안에 id를 포함한 이미지를 넣어서 스타일 가능하게 만드세요:

    ![screenshot](sunrise-sun-image.png)

+ 이미지가 너무 크네요. `style.css` 로 가서 다음 CSS를 더해 이미지 높이를 정하세요:

    ![screenshot](sunrise-sun-height.png)

    비율을 맞추기 위해 넓이는 자동으로 맞춰진다는데 유의해주세요.

+ 마지막으로 태양의 위치를 지정한 코드를 넣읍시다:

    ![screenshot](sunrise-sun-position.png)


## 프로젝트를 저장하세요 {.save}

# 2 단계: 일출 연출하기 { .activity}

일출을 연출하기 위해선 태양이 어떻게 움직이는 가와 얼마나 올라오는데 얼마나 오래 걸리는지를 지정 해야합니다.

그렇게 하기위해선 __key frames__리스트를 정의 해야합니다. 각 키 프레임은 요소의 CSS 속성을 애니메이션의 특정한 지점마다 정의해줍니다.

## 단계별 체크리스트 { .check}

+ 먼저 `@keyframes`을 사용해서 sunrise 라는 새 애니메이션을 만들어야 합니다. 

    이 CSS 코드를 `style.css` 파일 마지막에 더해주세요:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    이 코드는 태양 애니메이션이 시작할 때(`0%`) 와 끝(`100%`)에 태양의 위치를 지정합니다.

    태양이 하늘 `div`안에 있기 때문에 지정하는 `top` 과 `left` 위치는 하늘 안에 있습니다. `top: 100%` 가 웹페이지의 바닥이 아닌 하늘의 바닥 쪽이죠.


+ 이제 일출 애니메이션이 만들어졌으니 태양 이미지가 사용하도록 만들기만 하면 됩니다.

    다음 강조된 코드를 태양의 CSS에 더해주세요:

    ![screenshot](sunrise-sunrise.png)

    이 CSS는 태양 이미지가 일출 애니메이션을 10초동안 돌리게 만듭니다.

+ 트링켓에서 애니메이션을 다시 한번 보려면 **Autorun**을 클릭하세요. 

## 프로젝트를 저장하세요 {.save}

##도전과제: 대각 애니메이션 {.challenge}
일출 애니메이션에 코드를 더해 하늘 왼쪽 바닥에서 시작해서 대각선으로 중간쯤 맨 위로 가게 만들 수 있나요?

`left` 속성을 사용하면 됩니다. 예를 들자면:

```
left: 40%;
```

![screenshot](sunrise-left.png)

## 프로젝트를 저장하세요 {.save}


# 3 단계: 무한 반복하는 애니메이션 { .activity}

이 애니메이션을 무한하게 반복하게 만들어 봅시다.

## 단계별 체크리스트 { .check}

+ 일출 후 일몰하게 만들려면 애니메이션에 키프레임을 더해보세요:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    이건 애니메이션의 시작과 끝에 태양이 하늘 바닥에 있고 애니메이션의 33%에서 66%까진 최상단에 있다는 의미입니다.

+ 이제 `#sun` 애니메이션에 `infinite`란 단어를 더해서 영원히 반복되게 만들면 됩니다:

    ![screenshot](sunrise-infinite.png)

+ 애니메이션을 확인해보세요. 태양이 계속해서 떴다 지나요? 


## 프로젝트를 저장하세요 {.save}

# 4 단계: 하늘에 애니메이션 넣기 { .activity}

애니메이션은 움직임을 주는 데만 사용하지 않습니다. 하늘에 밤엔 어둡게 만드는 애니메이션을 줍시다.

## 단계별 체크리스트 { .check}

+ CSS에 `sky`란 애니메이션을 더하세요:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    이번엔 위치가 아닌 하늘의 색에 애니메이션을 준다는데 유의해주세요.

+ 하늘이 새 애니메이션을 사용하게 코드를 넣으세요:

    ```
    animation: sky 10s;
    ```

    ![screenshot](sunrise-sky.png)

+ **Autorun** 을 눌러서 애니메이션을 확인해보세요.

## 프로젝트를 저장하세요 {.save}

##도전과제: 하늘 개선하기 {.challenge}

하늘 애니메이션을 개선해서 태양에 맞춰 낮엔 푸르고 태양이 지면서 어둡게 만들 수 있나요? 하늘 애니메이션도 무한 반복하게 만드세요.

![screenshot](sunrise-sky-challenge.png)

##도전과제: 더 많은 애니메이션 {.challenge}

다른 이미지에 애니메이션을 더할 수 있나요? 위치, 색, 모양, 크기, 투명도 혹은 생각나는 무엇이던 애니메이션으로 더해볼 수 있습니다. 또한 애니메이션이 돌아가는 시간을 바꿔보세요.

애니메이션을 줄 각 아이템엔 다음과 같은 단계가 필요합니다:

+ HTML에 id와 함께 넣기
+ id에 스타일 더하기
+ @keyframes rule 만들기
+ 스타일에 `animation:` 을 사용해서 @keyframe으로 지정한 애니메이션 사용하기

이미지 아이콘을 눌러서 프로젝트에 포함된 다른 이미지들을 확인해보세요:

![screenshot](sunrise-images.png)

또한 원하는 이미지를 직접 업로드 해도 됩니다.

하늘이 아니라 바다에도 아이템들을 더할 수 있다는 점을 기억하세요.

![screenshot](sunrise-boat.png)

다음 예에선 무지개에 투명도 효과를 줘서 희미해지게 보이는 효과를 줍니다:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

보트는 시작점을 음수로 지정해서 애니메이션의 일부동안은 안보이게 만듭니다:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## 프로젝트를 저장해주세요 {.save}
