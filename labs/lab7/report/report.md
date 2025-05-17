---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Математическое моделирование"
author: "Волгин Иван Алексеевич"

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
lot: false # List of tables
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Изуяить и смоделировать математическую модель о эпидемии.

# Задание

1. Изучить задачу о эпидемии.
2. Построить модель о эпидемии с использованием Julia.
3. Построить модель о эпидемии OpenModelica.

# Выполнение лабораторной работы

1. Для начала я прочитал теоретическое введение в задачу о эпидемии и в ник в ее суть.

2. Далее я перешел к построению модели с использованием Julia. Сначала я решил вариант задачи, когда кол-ов заболевших меньше или равно порогового значения (I(0) <= I*). Я написал код решения на Julia (рис. [-@fig:001]) и получил график (рис. [-@fig:002]). 

![Код реализации задачи I(0) <= I*](image/1.png){#fig:001 width=70%}

![График эпидемии I(0) <= I*](image/2.png){#fig:002 width=70%}

Затем я все еще на Julia построил я написал реализацию задачи о эпидемии, при условии что кол-ов заболевших больше порогового значения (I(0) > I*) (рис. [-@fig:003]) и получил следующий график (рис. [-@fig:004]).

![Код реализации задачи I(0) > I*](image/3.png){#fig:003 width=70%}

![График эпидемии I(0) > I*](image/4.png){#fig:004 width=70%}

3. Затем я перешел в OpenModelica и сделал тоже самое, чтобы потом сравнить результаты. Сначала я написал код для I(0) <= I* (рис. [-@fig:005]) и получил идентичный график (рис. [-@fig:006]). 

![Код реализации задачи I(0) <= I*](image/5.png){#fig:005 width=70%}

![График эпидемии I(0) <= I*](image/6.png){#fig:006 width=70%}

После этого реализовал модель задачи для I(0) > I* (рис. [-@fig:007]) и снова получил полностью идентичный графак (рис. [-@fig:008]), что свидетельствует о правильности выполнения задачи.

![Код реализации задачи I(0) > I*](image/7.png){#fig:007 width=70%}

![График эпидемии I(0) > I*](image/8.png){#fig:008 width=70%}

# Выводы

В ходе выполнения данной лабораторной работы я изучил и реализовал задачу о эпидемии с помощью Julia и в OpenModelica.
