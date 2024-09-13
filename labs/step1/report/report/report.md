---
## Front matter
title: "Отчёт по этапу №1 индивидуального проекта"

subtitle: "Установка Kali Linux"
author: "Хусаинова Динара Айратовна, 

НПИбд-02-21, 1032212283"

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

Установить Kali Linux.

# Теоретическое введение

Kali Linux - это дистрибутив Linux на базе Debian с открытым исходным кодом, предназначенный для решения различных задач информационной безопасности, таких как тестирование на проникновение, исследования в области безопасности, компьютерная экспертиза и обратный инжиниринг[1].

# Выполнение этапа

## Установка Kali Linux

![Создание новой виртуальной машины](image/1.png){ #fig:001 width=70% height=70% }

![Выбор образа](image/11.png){ #fig:002 width=70% height=70% }

![Созданная и настроенная витуальная машина](image/111.png){ #fig:111 width=70% height=70% }


![Установка](image/3.png){ #fig:003 width=70% height=70% }

![Имя пользователя и задание пароля](image/4.png){ #fig:004 width=70% height=70% }

![Вход в систему](image/5.png){ #fig:005 width=70% height=70% }

![Интерфейс](image/6.png){ #fig:006 width=70% height=70% }

# Вывод

Успешно установлен Kali Linux.

# Список литературы. Библиография

[1] Документация по Kali Linux: https://www.kali.org/