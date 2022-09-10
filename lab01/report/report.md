---
# Front matter
lang: ru-RU
title: "Лабораторная работа №1"
subtitle: "Информационная безопасность"
author: "Доре Стевенсон Эдгар"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

1. Приобретение практических навыков установки операционной системы на виртуальную машину;

2. Настройки минимально необходимых для дальнейшей работы сервисов.

# Выполнение лабораторной работы


## Выполнение задания


Для установки на виртуальную машину VirtualBox операционной системы Linux (дистрибутив CentOS) в нашем случае использовалась внешняя операционная система Windows. 

В VirtualBox нажимаем "Машина" - "Создать" и задаем имя "Base для нашей будущей операционной системы. Тип - Linux, версия - Red Hat (64-bit).

![Имя и тип ОС](image/1.png){ #fig:001 width=70% }

Задаем объем оперативной памяти 6366МБ (Из 16384МБ возможных)

![Объем памяти](image/2.png){ #fig:002 width=70% }

Создадим новый динамический виртуальный жесткий диск, укажем тип VDI, выделим 25ГБ.

![Создание виртуального жесткого диска](image/3.png){ #fig:003 width=70% }

![Тип виртуального жесткого диска](image/4.png){ #fig:004 width=70% }

![Формат хранения](image/5.png){ #fig:005 width=70% }

![Размер виртуального жесткого диска](image/6.png){ #fig:006 width=70% }

Первоначальные основные настройки виртуальной машины заданы, теперь запускаем нашу операционную систему, выбираем образ дистрибутива CentOS. 

Теперь стали доступны варианты непосредственно установки дистрибутива и продолжение загрузки в тестовом режиме без установки. В дальнейшем нам необходимо будетпользоваться данной операционной системой, устанавливать приложения, сохранять файлы, поэтому выбираем пункт установки.

![Окно установки CentOS](image/7.png){ #fig:007 width=70% }

Отобразился обзор установки, где мы можем задать настройки уже нашей операционной системы: задать язык раскладки, пароль для суперпользователя, выбрать часовой пояс и другие. 

Выбираем русский язык, где это возможно, указываем ранее созданный виртуальный жесткий диск для системы и нажимаем "Начать установку".

![Обзор установки с настройками ОС](image/8.png){ #fig:008 width=70% }

После установки необходимо принять лицензию и по желанию создать пользователей.

Теперь можно завершать установку и переходить в CentOS.

![Лицензирование и создание пользователя](image/9.png){ #fig:009 width=70% }


В итоге получили готовую к использованию операционную систему Linux (дистрибутив CentOS) с установленными дополнениями гостевой ОС, что позволяет менять разрешение экрана, использовать двунаправленный буфер обмена с внешней ОС и др.

![ОС с установленными дополнениями гостевой ОС](image/12.png){ #fig:012 width=70% }

# Выводы

1. Приобрел практические навыки установки операционной системы на виртуальную машину;

2. Настроил минимально необходимые для дальнейшей работы сервисы.