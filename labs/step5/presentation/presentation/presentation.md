---
## Front matter
lang: ru-RU
title: "Этап №5 индивидуального проекта"
subtitle: "Использование Burp Suite"
author: " Хусаинова Д.А. Группа НПИбд-02-21 "


## i18n babel
babel-lang: russian 
babel-otherlangs: english 
mainfont: Arial 
monofont: Courier New 
fontsize: 12pt

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Цель

Научиться использовать Burp Suite.

# Выполнение лабораторной работы

Запускаю локальный сервер, на котором открою веб-приложение DVWA для тестирования инструмента Burp Suite

![Запуск локального сервера](image/1.PNG){#fig:001 width=70%}

# Выполнение лабораторной работы

Запускаю инструмент Burp Suite

![Запуск приложения](image/2.PNG){#fig:002 width=70%}

# Выполнение лабораторной работы

Открываю сетевые настройки браузера, для подготовке к работе 

![Сетевые настройки браузера](image/3.PNG){#fig:003 width=70%}

# Выполнение лабораторной работы

Изменение настроек сервера для работы с proxy и захватом данных с помощью Burp Suite 

![Настройки сервера](image/4.PNG){#fig:004 width=70%}

# Выполнение лабораторной работы

Изменяю настройки Proxy инструмента Burp Suite для дальнейшей работы 

![Настройки Burp Suite](image/5.PNG){#fig:005 width=70%}

# Выполнение лабораторной работы

Во вкладке Proxy устанавливаю "Intercept is on" 

![Настройки Proxy](image/6.PNG){#fig:006 width=70%}

# Выполнение лабораторной работы

Чтобы Burp Suite исправно работал с локальным сервером, наобходимо установить параметр `network_allow_hijacking_loacalhost` на `true`

![Настройки параметров](image/7.PNG){#fig:007 width=70%}

# Выполнение лабораторной работы

Пытаюсь зайти в браузере на DVWA, тут же во вкладки Proxy появляется захваченный запрос. Нажимаем "Forward", чтобы загрузить страницу 

![Получаемые запросы сервера](image/8.PNG){#fig:008 width=70%}

# Выполнение лабораторной работы

Загрузилась страница авторизации, текст запроса поменялся

![Страница авторизации](image/9.PNG){#fig:009 width=70%}

# Выводы

При выполнении лабораторной работы научилась использовать инструмент Burp Suite.

# Библиография

1. Документация по DVWA: https://kali.tools/?p=1820