---
## Front matter
title: "Отчёт по этапу №5 индивидуального проекта"

subtitle: "Использование Burp Suite"
author: "Хусаинова Динара Айратовна, НПИбд-02-21, 1032212283"

babel-lang: russian 
babel-otherlangs: english 
mainfont: Arial 
monofont: Courier New 
fontsize: 12pt

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---
# Цель работы

Научиться использовать Burp Suite.

# Теоретическое введение

Burp Suite представляет собой набор мощных инструментов безопасности веб-приложений, которые демонстрируют реальные возможности злоумышленника,
проникающего в веб-приложения. Эти инструменты позволяют сканировать,
анализировать и использовать веб-приложения с помощью ручных и автоматических методов. Интеграция интерфейсов этих инструментов обеспечивает полную
платформу атаки для обмена информацией между одним или несколькими инструментами, что делает Burp Suite очень эффективной и простой в использовании
платформой для атаки веб-приложений. [@parasram].

# Выполнение лабораторной работы

Запускаю локальный сервер, на котором открою веб-приложение DVWA для тестирования инструмента Burp Suite (рис. [-@fig:001]).

![Запуск локального сервера](image/1.PNG){#fig:001 width=70%}

Запускаю инструмент Burp Suite (рис. [-@fig:002]).

![Запуск приложения](image/2.PNG){#fig:002 width=70%}

Открываю сетевые настройки браузера, для подготовке к работе (рис. [-@fig:003]).

![Сетевые настройки браузера](image/3.PNG){#fig:003 width=70%}

Изменение настроек сервера для работы с proxy и захватом данных с помощью Burp Suite (рис. [-@fig:004]).

![Настройки сервера](image/4.PNG){#fig:004 width=70%}

Изменяю настройки Proxy инструмента Burp Suite для дальнейшей работы (рис. [-@fig:005]).

![Настройки Burp Suite](image/5.PNG){#fig:005 width=70%}

Во вкладке Proxy устанавливаю "Intercept is on" (рис. [-@fig:006]).

![Настройки Proxy](image/6.PNG){#fig:006 width=70%}

Чтобы Burp Suite исправно работал с локальным сервером, наобходимо установить параметр `network_allow_hijacking_loacalhost` на `true` (рис. [-@fig:007]).

![Настройки параметров](image/7.PNG){#fig:007 width=70%}

Пытаюсь зайти в браузере на DVWA, тут же во вкладки Proxy появляется захваченный запрос. Нажимаем "Forward", чтобы загрузить страницу (рис. [-@fig:008]).

![Получаемые запросы сервера](image/8.PNG){#fig:008 width=70%}

Загрузилась страница авторизации, текст запроса поменялся (рис. [-@fig:009]).

![Страница авторизации](image/9.PNG){#fig:009 width=70%}

История запросов хранится во вкладке Target.


# Выводы

При выполнении лабораторной работы научилась использовать инструмент Burp Suite.

# Список литературы. Библиография

[1] Документация по DVWA: https://kali.tools/?p=1820