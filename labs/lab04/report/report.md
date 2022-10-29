---
## Front matter
title: "Лабораторная работа №3"
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

Освоение процедуры оформления отчетов с помощью
легковесного языка разметки Markdown.

# Задание

1. В соответствующем каталоге сделайте отчёт по лабораторной работе No 3
в формате Markdown. В качестве отчёта необходимо предоставить отчёты
в 3 форматах: pdf, docx и md.
2. Загрузите файлы на github

# Теоретическое введение



# Выполнение лабораторной работы

Открываем терминал и переходим в каталог курса сформмированный при выполнении лабораторной работы №3
![Рис. 1](/home/ddobinali/Изображения/Снимки экрана/lab3.gitPull.png){ #fig:001 width=90% }

Переходим в каталог с шаблоном лабораторной работы №4, проводим компилялцию шаблона 
![Рис. 2](/home/ddobinali/Изображения/Снимки экрана/lab3.make.png){ #fig:001 width=90% }

Удаляем полученный файл
![Рис. 3](/home/ddobinali/Изображения/Снимки экрана/lab3.makeClean.png){ #fig:001 width=90% }

Открываем файл report.md с помощью текстого редактора gedit 
![Рис. 4](/home/ddobinali/Изображения/Снимки экрана/lab3.geditReportmd.png){ #fig:001 width=90% }

Загрузим файлы на github
!Рис. 5] (/home/ddobinali/Изображения/Снимки экрана/lab3.gitAdd.png) { #fig:001 width=90% }
# Выводы

Мы научились работать с Makefile и смогли сделать отчет с помощью Markdownn

# Список литературы{.unnumbered}

::: {#refs}
:::
