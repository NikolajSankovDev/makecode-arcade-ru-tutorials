# Поздравительная открытка
### @explicitHints true


## {Введение @showdialog}

Следуйте этим быстрым шагам, чтобы создать поздравительные открытки, которыми вы сможете поделиться с друзьями и семьей!

![Greetings](/static/skillmap/story/story1.gif "Happy birthday to you!" )



## {Шаг 2}

**Установить фон**

---

- :tree: Из категории ``||scene:Сцена||`` на панели инструментов:
схватить
```block
scene.setBackgroundImage(img`.`)
```
и перетащите его в пустой <br/>.
``||loops(noclick):при запуске||``<br/>
контейнер в рабочей области.

~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![The background gallery](/static/skillmap/story/choose-bg.gif "Toggle between editor and gallery" )
hint~

<br/><br/>

- :right arrow: Нажмите **Далее**, чтобы перейти к следующему шагу.


#### ~ tutorialhint

```blocks
//@highlight
scene.setBackgroundImage(img`.`)
```




## {Шаг 3}


- :paint brush: Нажмите на пустой серый квадрат внутри.
```block
scene.setBackgroundImage(img`.`)
```
чтобы открыть **редактор изображений**. <br/><br/>
Вы можете нарисовать свой собственный фон или выбрать его из **Галереи**.
![This is where the gallery is located](/static/skillmap/assets/gallery.png "You can switch over to the gallery or make your own image." )


~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![The background gallery](/static/skillmap/story/story-bg-select.gif "Toggle between editor and gallery" )
hint~


#### ~ tutorialhint

```blocks
//@highlight
scene.setBackgroundImage(storySprites.halloween)
```





## {Шаг 4}

**Посмотрите на свою карту.**

- :binoculars: Посмотрите на окно игры. <br/><br/>
Вы видите фон, который выбрали?




## {Шаг 5}

**Добавьте сердечное приветствие**<br/>
💛 💛 💛

---

- :ticket: Из категории ``||carnival:Carnival||`` перетащите
```block
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
```
в **конец** <br/>
``||loops(noclick):при запуске||``<br/>
контейнер, который уже находится в рабочей области.


- :mouse pointer: Измените сообщение на любое, какое захотите.


~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![The background gallery](/static/skillmap/story/step5.gif "Toggle between editor and gallery" )
hint~



#### ~ tutorialhint

```blocks
scene.setBackgroundImage(storySprites.halloween)
//@highlight
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)

```





## {Шаг 6}

**Изменить цвет текста**<br/>
🎨 🎨 🎨

---

- :mouse pointer: Если вы хотите изменить цвет текста, щелкните знак плюса (+) внутри
```block
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
```
и выберите любой цвет, который вам нравится.


~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![Click the plus to choose a color](/static/skillmap/story/step6.gif "Choose a color" )
hint~



#### ~ tutorialhint

```blocks
scene.setBackgroundImage(storySprites.halloween)
//@highlight
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top, 1)

```



## {Шаг 7}

**Время для пиццы**<br/>
🎉🎉🎉

---

- :tree: Откройте категорию ``||scene:Сцена||`` и перетащите
```block
effects.confetti.startScreenEffect()
```
в **конец** <br/>
``||loops(noclick):при запуске||``<br/>
контейнер, который уже находится в рабочей области.


- :mouse pointer: Измените эффект на любой желаемый.

~hint Нажмите здесь, чтобы узнать, как это сделать 🕵🏽

---

![Add an effect from the scene category](/static/skillmap/story/step7.gif "Choose an effect" )
hint~

#### ~ tutorialhint

```blocks
scene.setBackgroundImage(storySprites.halloween)
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
//@highlight
effects.confetti.startScreenEffect()

```




## {Шаг 8}

**Посмотрите на свое творение!**

- :binoculars: Посмотрите на окно игры. Карта выглядит так, как вы хотите?  <br/><br/>
Не стесняйтесь менять его, пока он вас не устроит.





## {Заканчивать}

**Поздравляем, вы закончили поздравительную открытку!**<br/>
🥳 🥳 🥳



~hint Как мне поделиться своей картой?💡

---

**Хотите поделиться своим проектом?**

Нажмите «Готово», чтобы вернуться к карте навыков, затем найдите в правом нижнем углу кнопку «Поделиться».

![Share your card](/static/skillmap/assets/share.gif )

hint~



Нажмите **Готово**, чтобы вернуться на главную страницу карты навыков, где вы сможете продолжить создание еще более подробной карты.



```blockconfig.global
carnival.addLabelTo("You Are Awesome", carnival.Areas.Top)
```



```package
carnival=github:microsoft/arcade-carnival#v0.0.7
```


```ghost
scene.setBackgroundColor(1)
scene.setBackgroundImage(img`.`)
effects.confetti.startScreenEffect()
carnival.addLabelTo("You Are Awesome", carnival.Areas.Bottom)
music.startSong(assets.song`birthday`, false)
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
