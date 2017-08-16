---
title: Будуємо робота
level: HTML & CSS 2
language: uk-UA
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Вступ {.intro}

У цьому проекті ви навчитесь як розташовувати зображення, щоб створити власного робота!

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-final.png)

# Крок 1: Даємо роботу очі {.activity}

Наділімо нашого робота очима!

## Список дій {.check}

+ Відкрийте редактор: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>. Якщо ви читаєте це онлайн, то також можете використати версію, яка вбудована нижче.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b29b50e571" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Кожне зображення в цьому проекті має свою назву (або **id**). Наприклад, HTML для зображення обличчя та очей ("face","eyes1" і "eyes2", які починаються в 8 рядку вашого коду) виглядають так:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

+ Ви можете використати id зображення, щоб створити власний стиль, для цього треба застосовати символ `#`. Це дозволить вам спроектувати кожну картинку окремо.

Натисніть на файл `style.css`. Звернули увагу, як відрізняється розмір обличчя робота та інших зображень?

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-id.png)

+ Додайте цей CSS код, щоб сформувати очі робота:

    #eyes1 {
        width: 200px;
    }
    

Зауважте, що ви створюєте лише зображення `eyes1`, за допомогою `#eyes1` у вашому CSS. Замість нього можна ще використати `#eyes2` або `#eyes3`!

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-eyes-width.png)

+ Звернули увагу, що кожна картинка зображена одна за одною? Це називається **відносним** розташуванням. Якщо вам потрібно ввести у браузер точне місце розташування очей робота, тоді замість відносного застосуйте **абсолютне** (absolute) розташування.

Додайте цих 3 рядки коду до CSS для вашого зображення `eyes1`:

    position: absolute;
    top: 200px;
    left: 100px;
    

Ви маєте побачити, що очі вашого робота розмістились у потрібному місці.

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-eyes-position.png)

Даний CSS код повідомляє браузеру наскільки далеко від верху веб-сторінки та від її лівої сторони має бути розташоване зображення.

![скріншот](robot-eyes-position2.png)

Ви зможете використовувати `bottom` замість `top`, щоб встановити розташування очей відносно низу екрану, а для правого боку `right` замість `left`.

# Крок 2: Даємо роботу посмішку {.activity}

Давайте створимо нашому роботу рот, щоб він міг посміхатись!

## Список дій {.check}

+ Додайте наступний CSS код, щоб створити роботу рот `mouth1` (мовою програми):

    #mouth1 {
        width: 50px;
        position: absolute;
        top: 200px;
        left: 200px;
    }
    

+ Рот вашого робота виглядає досить маленьким і знаходиться не там, де потрібно.

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-mouth.png)

Чи зможете ви це виправити, якщо внесете зміни у вашу CSS?

## Збережіть свій проект {.save}

## Завдання: створіть власного робота {.challenge}

Використовуйте отримані знання, щоб закінчити проектування свого робота. Нижче наведено декілька прикладів того, як він може виглядати:

![скріншот](https://raw.githubusercontent.com/RaspberryPiFoundation/webdev-curriculum/master/en-GB/Build%20a%20Robot/robot-examples.png)

## Збережіть свій проект {.save}

## Завдання: додайте свої власні зображення {.challenge}

Чи зможете ви знайти додаткові зображення, щоб прикріпити до робота та додати їх на свою веб-сторінку? Більше того, можна замінити обличчя робота на будь яке інше!

    <img id="face" src="myFace.png">
    

## Збережіть свій проект {.save}