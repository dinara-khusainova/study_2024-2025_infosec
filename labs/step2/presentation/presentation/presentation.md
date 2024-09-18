---
## Front matter
lang: ru-RU
title: "Этап №2 индивидуального проекта"
subtitle: "Установка DVWA"
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

# Цель работы

Установить DVWA.

# Задание

1. Установить DVWA.

# Теоретическое введение

Damn Vulnerable Web Application (DVWA) — это веб-приложение на PHP/MySQL, которое содержит различные уязвимости [1].

# Выполнение этапа 

# Репозиторий для скачивания

![Вход на репозиторий для скачивания DVWA](image/0.png){ #fig:006 width=70% height=70% }

# Выполнение команды wget

![Выполнение команды wget https://raw.githubusercontent.com/IamCarron/DVWA-Script/main/Install-DVWA.sh](image/1.png){ #fig:001 width=70% height=70% }

# Исполняемый скрипт. Запуск скрипта

![Делаем скрипт исполняемым и запускаем скрипт от имени root](image/2.png){ #fig:002 width=70% height=70% }

# Загрузка 

![Загрузка](image/3.png){ #fig:003 width=70% height=70% }

# SQL пользователь

![Ввод учетных данных для sql пользователя](image/4.png){ #fig:004 width=70% height=70% }

# Загрузка прошла успешно

![Конец загрузки](image/5.png){ #fig:005 width=70% height=70% }

# Вывод

В ходе выполнения первого этапа проекта успешно установлен DVWA.

# Библиография

1. Документация по DVWA: https://kali.tools/?p=1820