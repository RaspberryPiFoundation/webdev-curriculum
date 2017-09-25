---
제목:일출- 클럽 리더를 위한 노트
언어: ko-KR
embeds: "*.png" 
materials: [""]
...

#소개:
이 프로젝트에서 아이들은 CSS를 사용해 간단한 애니메이션을 만드는 방법을 배울 것입니다. 아이들은 CSS @keyframes rule을 사용해서 이미지와 div의 여러가지 속성들을 움직일 것입니다.

#온라인 소재 

[trinket](https://trinket.io/) 으로 HTML & CSS을 온라인으로 쓰는 걸 추천합니다. 이 프로젝트는 다음 트링켓을 포합하고 있습니다:

또한 이 빈 트링켓을 사용해서 [(jumpto.cc/trinket-blank)](http://jumpto.cc/trinket-blank) 직접 HTML & CSS를 쓰거나 이 템플릿 트링켓을 사용할 수 있습니다. [(jumpto.cc/trinket-template)](http://jumpto.cc/trinket-template).

또한 도전과제의 예시 해답을 가지고 있는 트링켓도 있습니다:

+ ['Sunrise' Finished](https://trinket.io/html/abcc0284a3)

#오프라인 소재
이 프로젝트는 원하신다면 [다음 링크에서](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/) 다운로드 받아 오프라인에서 끝낼 수 있습니다.이 프로젝트의 'Project Materials' 링크를 눌러 프로젝트 소재를 받을 수 있습니다. 이 링크엔 아이들이 프로젝트를 오프라인으로 완성하는데 필요한 소재가 포함된 'Project Resources' 란이 있습니다. 아이들이 각자 이 소재를 가지고 있도록 확인해주세요. 이 란엔 다음 파일이 포함되어 있습니다:

+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

'Club Leader Resources' 폴더에서 이 프로젝트의 완성본을 찾을 수 있고 다음을 포함하고 있습니다:

+ index.html
+ style.css
+ prefixfree.js
+ boat.png
+ sun.png
+ rainbow.png

#배움 목표s
+ CSS로 애니메이션과 스타일링 하기:
	+ 애니메이션의 단계를 정의하는 `@keyframes` rule 소개.
	+ 속성을 사용해서 웹페이지의 요소의 크기, 모양, 위치와 색깔정의하기.

#도전과제
+ "대각선 애니메이션" - 애니메이션 `@keyframe` 속성을 수정해서 왼쪽 사용하게 만들기:;
+ "하늘 개선하기" - keyframes 더 더하고 배경 만들기:.
+ "더 많은 애니메이션" - 여러가지 CSS 속성을 사용해서 이미지나 요소들 더 움직이기 만들어보기.

#자주 묻는 질문들

+ 이 프로젝트는 자바스크립트의 `prefixfree.js` 라이브러리를 사용하여 브라우저 사이에서 애니메이션의 호환을 가능하게 해줍니다. 이 라이브러리를 사용하지 않는다면 낡은 브라우저를 사용하는 아이들은 다음과 같이 브라우저에 애니메이션을 사용해야합니다:

```
animation: sky 10s infinite; 		  	//for all newer browsers
-webkit-animation: sky 10s infinite;  	// For Webkit browsers(Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// For Mozilla browsers
-o-animation: sky 10s infinite;       	// For Opera browsers
-ms-animation: sky 10s infinite;		// For Microsoft browsers 
```
