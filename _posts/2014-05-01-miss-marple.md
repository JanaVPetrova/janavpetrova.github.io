---
layout: post
comments: true
title:  Miss Marple
date:   2014-05-01 14:25:37
---

После редизайна проекта остается довольно много неиспользуемых файлов: партиалы, файлы css и js. Гугл подсказал
решение для [поиска неиспользуемых партиалов](https://github.com/vinibaggio/discover-unused-partials), но
для поиска ненужных ассетов ничего не нашлось. И сегодня я наконец-то закончила гем
[Miss Marple](https://github.com/JanaVPetrova/miss-marple), который выдает список неупомянутых в манифесте
файлов.

##### Как использовать:
Устанавливаем гем:

    $ gem install miss-marple

Переходим в директорию с Rails-проектом:

    $ cd my-rails-app

Запускаем:

    $ miss-marple

На выходе получаем список файлов, которые есть фактически и которые не были упомянуты в манифесте.
Ниже будет список файлов, в которых нашлись ключевые слова require или require_tree.

    Unused assets:
    /my-rails-app/app/assets/javascripts/unused

    Requiring files:
    /my-rails-app/app/assets/javascripts/application.js
    /my-rails-app/app/assets/stylesheets/application.css

Реквестирую фидбэк.:)