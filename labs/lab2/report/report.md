---
## Front matter
## Front matter
title: "Лабораторная работа №2"
subtitle: "Математическое моделирование"
author: "Волгин Иван"

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

Построить математическую модель для выбора правильной стратегии при решении задачи о погоне

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.


# Выполнение лабораторной работы

Построение модели (рис. [-@fig:001]).

![Код для построения модели](image/1.png){#fig:001 width=70%}

В итоге я получил вот такой рисунок (рис. [-@fig:002])

![Траектория катера](image/2.png){#fig:002 width=70%}

Отрисовываю движение катера с движением лодки и вижу, что траектории пересекаются (рис. [-@fig:003])

![совместные траектории](image/3.png){#fig:003 width=70%}

Вычисляю точку пересевения катера и лодки (рис. [-@fig:004])

![точка пересечения](image/4.png){#fig:004 width=70%}

Построение модели для второго случая (рис. [-@fig:005]).

![Код для построения модели второго случая](image/5.png){#fig:005 width=70%}

В итоге получаю такую траекторию (рис. [-@fig:006])

![Траектория катера](image/6.png){#fig:006 width=70%}

Отрисовываю движение катера с движением лодки для второго случая и вижу, что траектории пересекаются (рис. [-@fig:007])

![совместные траектории второго случая](image/7.png){#fig:007width=70%}

Вычисляю точку пересечения катера и лодки во втором случае (рис. [-@fig:008])

![точка пересечения](image/8.png){#fig:008 width=70%}

# Выводы

В процессе выполнения данной лабораторной работы я построил математическую модель для выбора правильной стратегии при решении задачи о погоне.

