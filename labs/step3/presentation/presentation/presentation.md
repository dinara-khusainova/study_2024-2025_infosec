---
## Front matter
lang: ru-RU
title: "Этап №3 индивидуального проекта"
subtitle: "Использование Hydra"
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

Приобретение практических навыков по использованию инструмента Hydra для брутфорса паролей.

# Задание

1. Реализовать эксплуатацию уязвимости с помощью брутфорса паролей.

# Теоретическое введение

- Hydra используется для подбора или взлома имени пользователя и пароля.
- Поддерживает подбор для большого набора приложений.

# Выполнение этапа 

# Файл паролей rockyou.txt

Чтобы пробрутфорсить пароль, нужно сначала найти большой список частоиспользуемых паролей. Его можно найти в открытых источниках, я взяла стандартный список паролей `rockyou.txt` для kali linux

![Распаковка архива со списком паролей](image/2.PNG){#fig:001 width=50%}

# Сайт DVWA

Захожу на сайт DVWA, полученный в ходе предыдущего этапа проекта. Для запроса hydra мне понадобятся параметры cookie с этого сайта

![Сайт, с которого получаем информацию о параметрах Cookie](image/1.PNG){#fig:002 width=50%}

# Hydra запрос

![Запрос Hydra](image/6.PNG){#fig:006 width=60%}

# Результат запроса 

![Результат запроса](image/3.PNG){#fig:003 width=70%}

# Ввод полученных данных на сайт для проверки

![Ввод полученного результата в уязвимую форму](image/4.PNG){#fig:004 width=70%}

# Результат проверки пароля

![Результат](image/5.PNG){#fig:005 width=70%}


# Вывод

Приобретены практические навыки по использованию инструмента Hydra для брутфорса паролей.

# Библиография

1. Документация по DVWA: https://kali.tools/?p=1820