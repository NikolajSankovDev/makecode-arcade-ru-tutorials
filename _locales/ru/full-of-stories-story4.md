# Самая короткая история
### @explicitHints true


## {Введение @showdialog}

Давайте воспользуемся тем, что мы узнали, и составим небольшой рассказ, которым поделимся с семьей и друзьями.

![Here's the story](/static/skillmap/story/story4.gif "Example of a page in our story." )


## {Шаг 2}

Прежде чем начать этот урок, придумайте историю.

Вы можете написать свою историю или использовать эту:

Жила-была ящерица, которая жила под мухомором.

По соседству на ромашке жила бабочка.

Каждый день бабочка пролетала мимо ящерицы и дразнила её с неба.

«Ха-ха! — говорила она. — Твой дом пахнет не так приятно, как мой».

Наконец однажды ящерица решила найти ромашку для себя.

Она пробовала снова и снова, но никак не могла устроиться удобно.

Что бы она ни делала, душистый цветок не делал её счастливой.

На следующий день ящерица вернулась к своему мухомору и жила долго и счастливо.





## {Шаг 3}


У вас есть своя история?

**Создайте свою первую страницу!** <br/>
📚 📖 📚

---

- :tree: Из ``||scene:Scene||``, привязка
```block
scene.setBackgroundImage(img`.`)
```
в **пустой**<br/>
``||loops(noclick):on start||`` <br/>
контейнер уже в рабочей области.


- :paint brush: **Нажмите на пустое поле изображения**, чтобы нарисовать первое изображение для своей истории.

💡 _Нет истории на примете? Вы можете использовать один из наших фонов._


#### ~ tutorialhint

```blocks
// @highlight
scene.setBackgroundImage(img`
9 9 9 9
9 9 9 9
7 7 7 7
`)
```




## {Шаг 4}

**Взгляните на экран игры.**

- :binoculars: Как выглядит ваше прошлое? Куда вы планируете добавить текст? Вершина? Середина? Нижний?




## {Шаг 5}

**✨ Отлично ✨**

Дайте читателю возможность насладиться вашим искусством, прежде чем накрывать его текстом.

- :redo: Из ``||loops: Loops||`` перетащите
```block
pause(1000)
```
его в **конец** <br/>
``||loops(noclick):on start||``<br/>
контейнер, который уже находится в рабочей области.


- :mouse pointer: Этот блок паузы останавливает программу на 1 секунду (1000 мс) перед переходом к следующей строке. Если вам нужно больше времени, вы можете изменить его на большее число.

#### ~ tutorialhint

```blocks
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
// @highlight
pause(1000)

```

## {Шаг 6}

Добавьте первую страницу текста.

---


- :circle: Из ``||game:Game||`` перетащите
```block
game.showLongText("Once upon a time...", DialogLayout.Bottom)
```
в **конец** <br/>
``||loops(noclick):on start||``<br/>
контейнер, который уже находится в рабочей области.


- :mouse pointer: Измените текст на тот, который будет служить первой строкой вашей истории. Вы также можете изменить расположение текста с ``||game(noclick):bottom||`` на другую область экрана.


💡 _Вы нашли другой способ добавить текст на другом уровне, который вам больше нравится? Не стесняйтесь использовать это вместо этого!_




#### ~ tutorialhint

```blocks
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
pause(1000)
//@highlight
game.showLongText("Once upon a time...", DialogLayout.Bottom)
```


## {Шаг 7}

**Создайте еще одну страницу!**

Добавьте еще один набор блоков с новой картинкой и новой строкой из вашей истории.

---

- :mouse pointer: Продолжайте добавлять наборы блоков, пока не дойдете до конца.
```block
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
pause(1000)
game.showLongText("Next door...", DialogLayout.Bottom)
```

💡 _Не всегда нужно добавлять блоки в одном и том же порядке.  Хотите показать несколько изображений без текста? Хотите изменить текст, не меняя картинку?  Поиграйте и посмотрите, что подойдет именно вам!_


#### ~ tutorialhint

```blocks
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("Once upon a time, there was a lizard who lived beneath a toadstool.", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("Next door, there lived a butterfly on a daisy.", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("Every day, the butterfly would sweep past and taunt the lizard from the sky.", DialogLayout.Bottom)
    game.showLongText("\"Ha ha!\" He would say. \"Your house doesn't smell as good as mine.\"", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("Finally, one day, the lizard decided to find a daisy of her own.", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(2000)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(2000)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(2000)
    game.showLongText("She tried and tried, but she just couldn't get comfortable.", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("No matter what she did, the fragrant flower didn't make her happy.", DialogLayout.Bottom)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    pause(1000)
    game.showLongText("The next day, the lizard moved back to her toadstool and lived happily ever after.", DialogLayout.Bottom)
    })
```


## {Шаг 8}

**Посмотрите, что у вас есть.**

- :binoculars: Не забывайте пролистывать свою историю во время сборки, чтобы убедиться, что время выбрано правильно.




## {Шаг 9}

**Нужны дополнительные действия?**<br/>
🎥 🎥 🎥

Вы можете использовать то, что узнали на последнем уровне, для добавления спрайтов в свою историю.

---

- :paper plane: Из ``||sprites:Sprites||``, возьмите
```block
let mySprite = sprites.create(img`
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    `, SpriteKind.Player)
```
и привяжите его к <br/>.
``||loops(noclick):on start||``<br/>
контейнер там, где это лучше всего подходит для вашей истории.


- :mouse pointer: Выберите свой спрайт, затем просмотрите категорию ``||sprites:Sprites||``, чтобы найти другие блоки, которые
позволит вам идеально расположить свой спрайт или добавить движение.




#### ~ tutorialhint

```blocks
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
    //@highlight
   let mySprite = sprites.create(img`
    ........................
    ............cc..........
    ............ccc.........
    ........ccc.ccccccc.....
    ........ccccc555555cc...
    ........ccb5555555555c..
    .....ccc.b55555ff15555c.
    .....cccb5555555ff55555c
    ......cb555555555555d55c
    ....c.b555555555bb55555c
    ....ccb555ddd5555b13bbc.
    ....ccd55ddddd555b3335c.
    .....cdd5ddddddd55b335c.
    ...c.bddddb555bbbd555c..
    ...ccdddddb555555bccc...
    ..cccddddddcc5555bcc....
    .cdccddddddddbcccbcccc..
    .cddbdddddddddbbbbc55c..
    .cdddddddddd55dbbbc5c...
    .cbddddbbbbd55ddbccc....
    ..cbdddbbbbd555dccc.....
    ...cccbbbbbbddd555c.....
    .....ccccccbd55555c.....
    ...........cc5555c......
    `, SpriteKind.Player)
    //@highlight
mySprite.setPosition(80, 90)
    pause(1000)
    game.showLongText("...happily ever after", DialogLayout.Bottom)

```




## {Шаг 10}

**👏 Долго и счастливо 👏**

Хотите сделать что-то особенное, чтобы закончить свою историю?

---

- :tree: Из ``||scene:Scene||``, возьмите
```block
effects.confetti.startScreenEffect()
```
и прикрепите его к **концу** <br/>
``||loops(noclick):on start||``<br/>
контейнер, который уже находится в рабочей области.


- :mouse pointer: Измените **конфетти** на то, что лучше всего подходит для вашей истории!


#### ~ tutorialhint

```blocks
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
   let mySprite = sprites.create(img`
    ........................
    ............cc..........
    ............ccc.........
    ........ccc.ccccccc.....
    ........ccccc555555cc...
    ........ccb5555555555c..
    .....ccc.b55555ff15555c.
    .....cccb5555555ff55555c
    ......cb555555555555d55c
    ....c.b555555555bb55555c
    ....ccb555ddd5555b13bbc.
    ....ccd55ddddd555b3335c.
    .....cdd5ddddddd55b335c.
    ...c.bddddb555bbbd555c..
    ...ccdddddb555555bccc...
    ..cccddddddcc5555bcc....
    .cdccddddddddbcccbcccc..
    .cddbdddddddddbbbbc55c..
    .cdddddddddd55dbbbc5c...
    .cbddddbbbbd55ddbccc....
    ..cbdddbbbbd555dccc.....
    ...cccbbbbbbddd555c.....
    .....ccccccbd55555c.....
    ...........cc5555c......
    `, SpriteKind.Player)
mySprite.setPosition(80, 90)
    pause(1000)
    game.showLongText("...happily ever after", DialogLayout.Bottom)
    //@highlight
    effects.bubbles.startScreenEffect()

```


## {Шаг 10}

**🎹 Звуковые эффекты 🎹**

Нужен ли вашей истории саундтрек?

---

- :mouse pointer: Из ``||music:Music||`` возьмите любой из <br/>
``||music: play [ ]||`` блокирует <br/>
и добавьте их в свой проект.


- :mouse pointer: Экспериментируйте со звуками и их размещением, чтобы добиться максимального эффекта.

#### ~ tutorialhint

```blocks
    //@highlight
    music.play(music.melodyPlayable(music.baDing), music.PlaybackMode.InBackground)
    scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
   let mySprite = sprites.create(img`
    ........................
    ............cc..........
    ............ccc.........
    ........ccc.ccccccc.....
    ........ccccc555555cc...
    ........ccb5555555555c..
    .....ccc.b55555ff15555c.
    .....cccb5555555ff55555c
    ......cb555555555555d55c
    ....c.b555555555bb55555c
    ....ccb555ddd5555b13bbc.
    ....ccd55ddddd555b3335c.
    .....cdd5ddddddd55b335c.
    ...c.bddddb555bbbd555c..
    ...ccdddddb555555bccc...
    ..cccddddddcc5555bcc....
    .cdccddddddddbcccbcccc..
    .cddbdddddddddbbbbc55c..
    .cdddddddddd55dbbbc5c...
    .cbddddbbbbd55ddbccc....
    ..cbdddbbbbd555dccc.....
    ...cccbbbbbbddd555c.....
    .....ccccccbd55555c.....
    ...........cc5555c......
    `, SpriteKind.Player)
mySprite.setPosition(80, 90)
    pause(1000)
    game.showLongText("...happily ever after", DialogLayout.Bottom)
    effects.bubbles.startScreenEffect()
})
```


## {Финал}

**🤣 Поздравляю 🤣**

Вы написали историю, которой можете гордиться!


~hint Как мне поделиться своей историей?💡

---

**Хотите поделиться своим проектом?**

Нажмите «Готово», чтобы вернуться к карте навыков, затем найдите в правом нижнем углу кнопку «Поделиться».

![Share your card](/static/skillmap/assets/share.gif )

hint~


Когда вы закончите читать свою историю, нажмите **Готово**, чтобы вернуться на главную страницу, где вы сможете поделиться ею со всеми, кого знаете!

```blockconfig.global
pause(1000)
let mySprite: Sprite = null
carnival.addLabelTo(" ", carnival.Areas.Top)
game.showLongText("Once upon a time...", DialogLayout.Bottom)
music.play(music.melodyPlayable(music.baDing), music.PlaybackMode.InBackground)
mySprite.setFlag(SpriteFlag.StayInScreen, true)

```

```package
carnival=github:microsoft/arcade-carnival#v0.0.7
arcade-storytelling=github:microsoft/arcade-storytelling/
arcade-animations=github:microsoft/arcade-character-animations
short-story-assets-2=github:kiki-lee/short-story-assets-2#v0.0.5
short-story-assets-1=github:kiki-lee/short-story-assets-1#v0.0.6
```

```ghost
music.stopAllSounds()
scene.setBackgroundColor(1)
pauseUntil(() => controller.anyButton.isPressed())
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
pause(1000)
game.showLongText("Once upon a time", DialogLayout.Bottom)
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
pause(1000)
game.showLongText("Finally, one day, the lizard decided to find a daisy of her own.", DialogLayout.Bottom)
scene.setBackgroundImage(img`
9 9 9 9 
9 9 9 9 
7 7 7 7 
`)
music.play(music.createSoundEffect(WaveShape.Sine, 5000, 0, 255, 0, 500, SoundExpressionEffect.None, InterpolationCurve.Linear), music.PlaybackMode.UntilDone)
music.play(music.createSong(hexhex`00780004080200`), music.PlaybackMode.InBackground)
let mySprite = sprites.create(img`.`, SpriteKind.Player)
story.printText(":)", 0, 0)
story.startCutscene(function () {
    story.spriteSayText(mySprite, ":)")
})
story.setPagePauseLength(1000, 1000)
story.printCharacterText("")
story.setSoundEnabled(false)
mySprite.sayText(" ")
game.splash("")
game.showLongText("", DialogLayout.Bottom)
carnival.addLabelTo("Whack-the-Mole", carnival.Areas.Top)
mySprite.setPosition(0, 0)
story.cancelCurrentCutscene()
story.cancelSpriteMovement(mySprite)
story.spriteMoveToLocation(mySprite, 0, 0, 100)
music.setVolume(20)
    music.play(music.createSong(hex`00780004080200`), music.PlaybackMode.UntilDone)
    music.play(music.stringPlayable("- - - - - - - - ", 120), music.PlaybackMode.UntilDone)
    music.play(music.melodyPlayable(music.baDing), music.PlaybackMode.UntilDone)
    music.play(music.createSoundEffect(WaveShape.Sine, 5000, 0, 255, 0, 500, SoundExpressionEffect.None, InterpolationCurve.Linear), music.PlaybackMode.UntilDone)
    music.stopAllSounds()
    animation.runImageAnimation(
mySprite,
[img`.`],
100,
true
)

characterAnimations.loopFrames(
mySprite,
[img`.`],
500,
characterAnimations.rule(Predicate.NotMoving)
)

mySprite.startEffect(effects.spray)
mySprite.setImage(img`.`)
scene.cameraShake(4, 500)
mySprite.setVelocity(-20, 0)
mySprite.x = 0
mySprite.setFlag(SpriteFlag.StayInScreen, false)
```

