---
## Front matter
title: "Отчёт по лабораторной работе №6"
subtitle: "НБИбд-04-22"
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

Освоение арифметических инструкций языка ассемблера NASM

# Задание

1. Выполнить работу с символьными и численными данными в NASM
2. Отработать на практике арифметические операции в NASM
3. Написать программу вычисления выражения с входными данными


# Выполнение лабораторной работы

Создаём каталог для этой лабораторной и создаём в нём файл lab6-1.asm

![Рис. 1](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_1.png?raw=true)

Введём код из листинга 7.1, который выведет значение регистра eax, скомпилируем его и проверим работу

![Рис. 2](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_3.png?raw=true)

Далее изменим и вместо символов запишем в регистр числа, скомпилируем полученный код и проверим результат

![Рис. 3](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_4.png?raw=true)

Создадим файл lab6-2.asm, введём туда код из листинга 7.2, и проверим результат работы программы.

![Рис. 4](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_5.png?raw=true)

Так же как и на прошлом шаге заменим символы на числа и проверим резульат

![Рис. 5](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_6.png?raw=true)

Теперь заменим функцию iprintLF на iprint. Теперь после вывода результата не создается новая строка

![Рис. 6](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_7.png?raw=true)

Создадим файл lab6-3.asm, куда введём код из листинга 7.3. Скомпилируем и проверим результат

![Рис. 7](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_8.png?raw=true)

Изменим код так, чтобы он вычислял выражение f(𝑥) = (4 ∗ 6 + 2)/5.

![Рис. 8](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7-13.png?raw=true)

Проверим результат работы программы

![Рис. 9](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_9.png?raw=true)

Теперь создадим файл variant.asm, в который вставим код из листинга 7.3, при помощи которого вычислим вариант самостоятельной работы

![Рис. 10](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_10.png?raw=true)

Напишем код, который решит уравнение 5 * (x + 18) - 28

![Рис. 11](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_12.png?raw=true)

Проверим корректность работы программы

![Рис. 12](https://github.com/ObinaliDenis/ODD_archpc/blob/master/labs/lab07/report/image/lab7_11.png?raw=true)

Ответы на вопросы лабораторной работы:
1. Какие строки листинга 7.4 отвеча-
ют за вывод на экран сообщения ‘Ваш вариант:’?
Ответ: mov eax,rem call sprint
2. Для чего используется следующие инструкции? 
Ответ:
nasm - создаёт объектный файл
mov ecx,x - запись переменной в регистр ecx
mov edx, 80 - запись размера переменной в регистр edx
call sread - вызов функции чтения данных
3. Для чего используется инструкция “call atoi”? 
Ответ: вызывает функции преобразующей ASCII код символа в число
4. Какие строки листинга 7.4 отвечают за вычисления варианта?
Ответ: 
xor edx,edx
mov ebx,20
div ebx
inc edx
5. В какой регистр записывается остаток от деления при выполнении ин-
струкции “div ebx”?
Ответ: ebx
6. Для чего используется инструкция “inc edx”
Ответ: величивает значение edx на 1.
7. Какие строки листинга 7.4 отвечают за вывод на экран результата вычис-
лений?
Ответ: 
mov eax,rem
call sprint
mov eax,edx
call iprintLF


# Выводы

В результате выполения лабораторной работы были освоены арифметические
инструкции языка ассемблера NASM

