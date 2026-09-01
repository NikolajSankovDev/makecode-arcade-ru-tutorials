# Большое приветствие
### @explicitHints true


## {Введение @showdialog}

Вы создали открытку, теперь давайте сделаем ее особенной!

![Send our love](/static/skillmap/story/story2.gif "Why do tropical fish like saltwater?" )


## {Шаг 2}

Код простой карты уже есть в рабочей области.<br/>
✉️ 💌 ✉️

---

- :mouse pointer: Вы можете добавить к этой карте или изменить ее на что-то совершенно другое.


💡 **Совет.** _Если ваш код не работает и вы не можете понять, почему, нажмите _<br/>
**"Заменить мой код"**<br/>
_чтобы заменить блоки в вашем рабочем пространстве новым стартовым кодом._



#### ~ tutorialhint
```blocks
scene.setBackgroundImage(storySprites.halloween)
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
effects.confetti.startScreenEffect()
```



## {Шаг 3}

Добавьте музыку, которая воспроизводится при нажатии кнопки **(A)**.

---

- :game: Из категории ``||controller:Контроллер||`` перетащите
```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    music.play(music.createSong(hex`00780004080200`), music.PlaybackMode.InBackground)
})
```
в **пустую область** рабочей области.


- :mouse pointer: Щелкните пустое серое поле, чтобы открыть музыкальный редактор и создать свою собственную песню!


~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![Add blocks to make music](/static/skillmap/story/step2-3.gif " " )

hint~


#### ~ tutorialhint
``` blocks
//@highlight
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    //@highlight
    music.play(music.createSong(hex`0078000408020108001c000e050046006603320000040a002d000000640014000132000201000244000000040002222c04000800012508000c000220250c00100002222a10001400031d242a14001800012518001c00021b221c002000012720002400012a24002800031d2427`), music.PlaybackMode.InBackground)
})
```




## {Шаг 4}

**Попробуйте.**

- :binoculars: Посмотрите в окно игры и нажмите кнопку **A** (или пробел), чтобы услышать музыку.

💡 _Возможно, вам придется включить звук рядом с окном игры, чтобы услышать добавленную вами музыку._


![Don't forget to turn on the sound]( /static/skillmap/assets/sound-on.gif "Image of the sound button to the right of the game window" )




## {Шаг 5}

**Какой приятный сюрприз**

Добавьте на свою открытку еще одно сообщение, чтобы выразить свою заботу.

---

- :circle: Из ``||game:Игра||``, возьмите
```block
    game.showLongText("To the greatest Earth I know", DialogLayout.Bottom)
```
и закрепите его **внизу** <br/>.
``||controller(noclick):когда кнопка [A] [нажата]||``<br/>
контейнер.


- :mouse pointer: Измените это сообщение, чтобы оно имело смысл с остальной частью вашего проекта.

~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![Add a message from the game category](/static/skillmap/story/step2-5.gif " " )
hint~

```blockconfig.local
game.showLongText("To the greatest Earth I know", DialogLayout.Bottom)
```

#### ~ tutorialhint
``` blocks

controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    music.play(music.createSong(hex`0078000408020108001c000e050046006603320000040a002d000000640014000132000201000244000000040002222c04000800012508000c000220250c00100002222a10001400031d242a14001800012518001c00021b221c002000012720002400012a24002800031d2427`), music.PlaybackMode.InBackground)

    //@highlight
    game.showLongText("Happy Earth Day", DialogLayout.Bottom)
})

```


## {Шаг 6}

**🎨 Сделайте это POP 🎨**<br/>
Настройте текстовый фрейм, чтобы объединить все это.

---

- :circle: Из ``||game:Игра||``, возьмите
```block
game.setDialogFrame(img`.`)
```
и закрепите его **вверху** <br/>.
``||controller(noclick):когда кнопка [A] [нажата]||``<br/>
контейнер, который уже находится в вашей рабочей области.


- :mouse pointer: Выберите дизайн, щелкнув пустое поле и выбрав его.
еще кое-что из **Галереи**.

~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![Change the frame](/static/skillmap/story/step2-6.gif " " )
hint~


#### ~ tutorialhint
``` blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    //@highlight
    game.setDialogFrame(sprites.dialog.mediumLeaf1)
    music.play(music.createSong(hex`0078000408020108001c000e050046006603320000040a002d000000640014000132000201000244000000040002222c04000800012508000c000220250c00100002222a10001400031d242a14001800012518001c00021b221c002000012720002400012a24002800031d2427`), music.PlaybackMode.InBackground)


    game.showLongText("Happy Earth Day", DialogLayout.Bottom)
    })

```



## {Шаг 7}

**Попробуйте еще раз.**

- :binoculars: Посмотрите на окно игры и нажмите кнопку
**Кнопка** (или пробел), чтобы увидеть текст и услышать музыку.





## {Шаг 8}

**Последний штрих 🎀**

Измените цвет текста, чтобы он хорошо сочетался с фоном.

---

- :circle: Из ``||game:Игра||``, возьмите
```block
game.setDialogTextColor(1)
```
и прикрепите его к **верхней части** <br/>.
``||controller(noclick):когда кнопка [A] [нажата]||``<br/>
блок в вашем рабочем пространстве.


- :mouse pointer: **Нажмите на образец цвета** и выберите цвет, который хорошо сочетается с вашим сообщением.  <br/><br/>
Ничего страшного, если вам придется изменить его несколько раз, прежде чем он будет выглядеть правильно.


~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![The background gallery](/static/skillmap/story/step2-8.gif "Toggle between editor and gallery" )
hint~


#### ~ tutorialhint
``` blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    //@highlight
    game.setDialogTextColor(1)
    game.setDialogFrame(sprites.dialog.mediumLeaf1)
    music.play(music.createSong(hex`0078000408020108001c000e050046006603320000040a002d000000640014000132000201000244000000040002222c04000800012508000c000220250c00100002222a10001400031d242a14001800012518001c00021b221c002000012720002400012a24002800031d2427`), music.PlaybackMode.InBackground)

    game.showLongText("Happy Earth Day", DialogLayout.Bottom)
    })
```



## {Шаг 9}

**Посмотрите на свою последнюю карточку.**

- :binoculars: Посмотрите на окно игры и нажмите кнопку
**Кнопка** (или пробел), чтобы увидеть, как теперь выглядит ваш текст.





## {Финал}

**✨ Поздравляю ✨**

Вы сделали открытку, которую будет рад получить любой друг!



~hint Как мне поделиться своей картой?💡

---

**Хотите поделиться своим проектом?**

Нажмите «Готово», чтобы вернуться к карте навыков, затем найдите в правом нижнем углу кнопку «Поделиться».

![Share your card](/static/skillmap/assets/share.gif )

hint~



Нажмите **Готово**, чтобы вернуться к основной карте навыков и поделиться своей карточкой с другом, а затем перейдите на следующий уровень, где вы придумаете шутку!


```blockconfig.global
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
game.showLongText("Happy Earth Day", DialogLayout.Bottom)
game.setDialogTextColor(1)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    music.play(music.createSong(hex`00780004080200`), music.PlaybackMode.InBackground)
})
```


```package
carnival=github:microsoft/arcade-carnival#v0.0.7
```


```template
scene.setBackgroundImage(storySprites.world)
carnival.addLabelTo("You Are Awesome", carnival.Areas.Bottom)
effects.confetti.startScreenEffect()
```

```ghost
scene.setBackgroundColor(1)
    game.setDialogTextColor(1)
    game.setDialogFrame(img`
        88888..8888888888888888....88888.
        87768888777877787778777888867778.
        87777686767876767678767688777778.
        87767767667676676676766786776768.
        8677676767767767677677678676778..
        .877768777686767776867678667768..
        .886668888888888888888888886688..
        .888888866666666666666668877768..
        88677786666666666666666668766778.
        87766686666666666666666668776678.
        87667786666666666666666668677778.
        87777686666666666666666668866888.
        88866886666666666666666668677778.
        87777686666666666666666668776678.
        87667786666666666666666668666778.
        87766786666666666666666668777688.
        88677786666666666666666668766778.
        87766686666666666666666668776678.
        87667786666666666666666668677778.
        87777686666666666666666668866888.
        88866886666666666666666668677778.
        87777686666666666666666668776678.
        87667786666666666666666668666778.
        87766786666666666666666668777688.
        .867778866666666666666668888888..
        .886688888888888888888888866688..
        .867766876768677767686777867778..
        .8776768767767767677677676767768.
        86767768766767667667676676776778.
        87777788676787676767876768677778.
        87776888877787778777877788886778.
        88888..88888888888888888....8888.
        .................................
        `)
    game.showLongText("You are so special", DialogLayout.Bottom)
```


```assetjson

{
  "README.md": " ",
  "assets.json": "",
  "images.g.jres": "{\n    \"song2\": {\n        \"data\": \"0078000408060107001c00020a006400f401640000040000000000000000000000000000000000a80000000200012504000600012508000c0001270e001000012514001800012a18001e00012920002200012524002600012528002c0001272e003000012534003800012c38003e00012a40004200012544004600012548004c0001314c005000012e50005200012a52005400012a54005600012956005800012958005a0001275a006200012762006600013068006c0001306e007400012e76007c00012a7e008000012c82008400012a\",\n        \"mimeType\": \"application/mkcd-song\",\n        \"displayName\": \"birthday\"\n    },\n    \"song1\": {\n        \"data\": \"0078000408020202001c00010a006400f40164000004000000000000000000000000000500000077000000040002423c0400080002413a08000c00023f380c001000023d3610001400023c3514001800023d3618001c00023f381c002000023c3522002400023d3624002600023f382600280002413a28002a00023d362a002e00023f3830003200023d3632003400023c3536003800023a333a004000023c3507001c00020a006400f401640000040000000000000000000000000000000000660000000200013004000600012e08000a00012c0c000e00012a10001200012914001600012a18001a00012c1c001e00012922002400012a24002600012c26002800012e28002a00012a2a002c00012c30003200012a3200340001293600380001273a003c000129\",\n        \"mimeType\": \"application/mkcd-song\",\n        \"displayName\": \"Noel Halls\"\n    },\n    \"*\": {\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"dataEncoding\": \"base64\",\n        \"namespace\": \"myImages\"\n    }\n}",
  "images.g.ts": "// Auto-generated code. Do not edit.\nnamespace myImages {\n\n    helpers._registerFactory(\"image\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"animation\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"song\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"song2\":\n            case \"birthday\":return hex`0078000408060107001c00020a006400f401640000040000000000000000000000000000000000a80000000200012504000600012508000c0001270e001000012514001800012a18001e00012920002200012524002600012528002c0001272e003000012534003800012c38003e00012a40004200012544004600012548004c0001314c005000012e50005200012a52005400012a54005600012956005800012958005a0001275a006200012762006600013068006c0001306e007400012e76007c00012a7e008000012c82008400012a`;\n            case \"song1\":\n            case \"Noel Halls\":return hex`0078000408020202001c00010a006400f40164000004000000000000000000000000000500000077000000040002423c0400080002413a08000c00023f380c001000023d3610001400023c3514001800023d3618001c00023f381c002000023c3522002400023d3624002600023f382600280002413a28002a00023d362a002e00023f3830003200023d3632003400023c3536003800023a333a004000023c3507001c00020a006400f401640000040000000000000000000000000000000000660000000200013004000600012e08000a00012c0c000e00012a10001200012914001600012a18001a00012c1c001e00012922002400012a24002600012c26002800012e28002a00012a2a002c00012c30003200012a3200340001293600380001273a003c000129`;\n        }\n        return null;\n    })\n\n}\n// Auto-generated code. Do not edit.\n",
  "main.blocks": "<xml xmlns=\"https://developers.google.com/blockly/xml\"><block type=\"pxt-on-start\" x=\"0\" y=\"0\"></block></xml>",
  "main.ts": "\n",
  "pxt.json": "{\n    \"name\": \"Untitled - Copy - Copy - Copy\",\n    \"description\": \"\",\n    \"dependencies\": {\n        \"device\": \"*\",\n        \"carnival\": \"github:microsoft/arcade-carnival#v0.0.7\"\n    },\n    \"files\": [\n        \"main.blocks\",\n        \"main.ts\",\n        \"README.md\",\n        \"assets.json\",\n        \"images.g.jres\",\n        \"images.g.ts\"\n    ],\n    \"targetVersions\": {\n        \"branch\": \"v1.11.21\",\n        \"tag\": \"v1.11.21\",\n        \"commits\": \"https://github.com/microsoft/pxt-arcade/commits/5fb4210ecb70e5d405aa1a5701b4408b5bfe9094\",\n        \"target\": \"1.11.21\",\n        \"pxt\": \"8.4.15\"\n    },\n    \"preferredEditor\": \"blocksprj\"\n}\n"
}

```