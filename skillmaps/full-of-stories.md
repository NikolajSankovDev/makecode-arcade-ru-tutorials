# Истории на любой вкус
* name: Истории на любой вкус
* description: Проявите творческие способности: создавайте поздравительные открытки, шутки и короткие истории.
* infoUrl: skillmap/educator-info/story-map-info
* bannerUrl: /static/skillmap/story/story-comp.png
* backgroundurl: /static/skillmap/backgrounds/story-comp.png
* primarycolor: #28f1f6
* secondarycolor: #fff53d
* tertiarycolor: #dfffff
* completednodecolor: #3b5c6c
* highlightcolor: #ffffff
* allowcodecarryover: true
* tags: легко, начинающие, руководства

## stories
* layout: manual

### story1
* allowcodecarryover: false
* name: Поздравительная открытка
* type: tutorial
* description: Сделайте красивую поздравительную открытку за несколько минут!
* url: https://github.com/NikolajSankovDev/makecode-arcade-ru-tutorials/skillmaps/full-of-stories/greeting-card
* imageUrl: /static/skillmap/story/story1.gif
* tags: легко, история, творчество, открытка
* next: story2
* position: 0 3

### story2
* name: Открытка с музыкой
* type: tutorial
* description: Добавьте музыку к открытке — получится подарок, который радует снова и снова!
* url: https://github.com/NikolajSankovDev/makecode-arcade-ru-tutorials/skillmaps/full-of-stories/bigger-greeting
* imageUrl: /static/skillmap/story/story2.gif
* tags: легко, открытка, музыка, искусство
* next: story3
* position: 1 2

### story3
* name: Время шуток
* allowcodecarryover: false
* type: tutorial
* description: Создайте первую историю в Arcade с помощью шутки из двух строк!
* url: https://github.com/NikolajSankovDev/makecode-arcade-ru-tutorials/skillmaps/full-of-stories/joking-around
* imageUrl: /static/skillmap/story/story3.gif
* tags: легко, история, шутка, поделиться
* next: story4
* position: 2 1

### story4
* name: Самая короткая история
* allowcodecarryover: false
* type: tutorial
* description: Запрограммируйте собственную короткую историю в MakeCode Arcade!
* url: https://github.com/NikolajSankovDev/makecode-arcade-ru-tutorials/skillmaps/full-of-stories/shortest-story
* imageUrl: /static/skillmap/story/story4.png
* tags: легко, история, поделиться
* next: beginner-cert-1
* position: 3 0

### beginner-cert-1
* name: Поздравляем!
* kind: completion
* type: certificate
* url: /static/skillmap/certificates/beginner-cert-01.pdf
* imageUrl: /static/skillmap/certificates/beginner-cert-01.png
* position: 4 -1
* actions:
    * map: [Попробовать Talent Show](/skillmap/star)
    * editor: [Открыть творческий режим](/)
* rewards:
    * certificate:
        * url: /static/skillmap/certificates/beginner-cert-01.pdf
        * preview: /static/skillmap/certificates/beginner-cert-01.png
    * completion-badge:
        * image: /static/badges/badge-story.png
        * name: Приветствия
