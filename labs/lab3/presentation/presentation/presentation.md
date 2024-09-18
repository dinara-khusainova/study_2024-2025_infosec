---
## Front matter
lang: ru-RU
title: "Лабораторная работа №3"
subtitle: "Дискреционное разграничение прав в Linux. Два пользователя"
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

Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей.

# Теоретическое введение

**Права доступа** определяют, какие действия конкретный пользователь может или не может совершать с определенным файлами и каталогами. С помощью разрешений можно создать надежную среду — такую, в которой никто не может поменять содержимое ваших документов или повредить системные файлы. [1]

**Группы пользователей Linux** кроме стандартных root и users, здесь есть еще пару десятков групп. Это группы, созданные программами, для управления доступом этих программ к общим ресурсам. Каждая группа разрешает чтение или запись определенного файла или каталога системы, тем самым регулируя полномочия пользователя, а следовательно, и процесса, запущенного от этого пользователя. Здесь можно считать, что пользователь - это одно и то же что процесс, потому что у процесса все полномочия пользователя, от которого он запущен. [2]

# Выполнение лабораторной работы

# Создание guest2 

![Добавление пользователя guest2](image/1.PNG){ #fig:001 width=70% height=70% }

# Добавление пользователя guest2 в группу guest 

![Добавление пользователя guest2 в группу guest](image/2.PNG){ #fig:002 width=70% height=70% }

# Сранение вывода команд

![Сранение вывода команд](image/3.PNG){ #fig:003 width=70% height=70% }

# Сравнение полученной информации с содержимым файла /etc/group

![Сравнение полученной информации с содержимым файла /etc/group](image/4.PNG){ #fig:004 width=70% height=70% }

# newgrp guest, chmod g+rwx /home/guest, chmod 000 dir1

![newgrp guest, chmod g+rwx /home/guest, chmod 000 dir1](image/5.PNG){ #fig:005 width=70% height=70% }

# Вывод

Были получены практические навыки работы в консоли с атрибутами файлов для групп пользователей

# Список литературы. Библиография

[0] Методические материалы курса

[1] Права доступа: https://codechick.io/tutorials/unix-linux/unix-linux-permissions

[2] Группы пользователей: https://losst.pro/gruppy-polzovatelej-linux#%D0%A7%D1%82%D0%BE_%D1%82%D0%B0%D0%BA%D0%BE%D0%B5_%D0%B3%D1%80%D1%83%D0%BF%D0%BF%D1%8B
