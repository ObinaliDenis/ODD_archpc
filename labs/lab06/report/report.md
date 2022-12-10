---
## Front matter
title: "Отчёт по лабораторной работе №5"
subtitle: "Архитектура вычислительных систем"
author: "Обинали Денис Джеральдович"

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
lot: true # List of tables
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
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков работы в Midnight Commander. Освоение
инструкций языка ассемблера mov и int.

# Задание


# Теоретическое введение


# Выполнение лабораторной работы

В Midnight commander перейдем в каталог arch-pc и создадим в нём каталог lab05(рис. [-@fig:001])

![Рис. 1](home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab5_1-3.png) { #fig:001 width=90% }

Откроем файл lab5-1.asm и введём текст из листинга 6.1

![Рис. 2](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab05_4-6.png) { #fig:001 width=90% }

Оттранслируем текст в объектный файл и проверим работу

![Рис. 3](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab5_7-8.png) { #fig:001 width=90% }

Скачаем и переместим файл in_out.asm в каталог lab05

![Рис. 4](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab05_9-10.png) { #fig:001 width=90% }

Создадим копию файла lab5-1.asm и назовём её lab5-2.asm

![Рис. 5](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab05_11.png) { #fig:001 width=90% }

Заменим текст на текст из листинга 6.2

![Рис. 6](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab06/report/image/lab05-12.png?raw=true) { #fig:001 width=90% }

Создадим исполняемый файл и проверим его работу

![Рис. 7](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab05_12-2.png) { #fig:001 width=90% }

Заменим подпрограмму sprintLF на sprint и проверим работу

![Рис. 8](/home/ddobinali/work/study/2022-2023/Архитектура компьютера/ODD_archpc/labs/lab06/report/image/lab05_13.png) { #fig:001 width=90% }
# Выводы

Я научился работе с MC и понял инструкции mov и int

# Список литературы{.unnumbered}

::: {#refs}
:::
