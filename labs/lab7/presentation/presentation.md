---
## Front matter
lang: ru-RU
title: Лабораторная работа №7
subtitle: Математическое моделирование
author:
  - Волгин И.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 17 мая 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Волгин Иван Алексеевич
  * Студент учебной группы НФИбд-01-22
  * Российский университет дружбы народов
  
:::
::::::::::::::

## Цель работы

Изуяить и смоделировать математическую модель о эпидемии.

## Задание

1. Изучить задачу о эпидемии.
2. Построить модель о эпидемии с использованием Julia.
3. Построить модель о эпидемии OpenModelica.

# Выполнение лабораторной работы

## Код реализации задачи I(0) <= I* на Julia и ее график

![](image/1.png){#fig:001 width=49%}
![](image/2.png){#fig:002 width=49%}

## Код реализации задачи I(0) > I* на Julia и ее график 

![](image/3.png){#fig:003 width=49%}
![](image/4.png){#fig:004 width=49%}

## Код реализации задачи I(0) <= I* в OpenModelica и ее график

![](image/5.png){#fig:005 width=49%}
![](image/6.png){#fig:006 width=49%}

## Код реализации задачи I(0) > I* в OpenModelica и ее график

![](image/7.png){#fig:007 width=49%}
![](image/8.png){#fig:008 width=49%}

## Выводы

В ходе выполнения данной лабораторной работы я изучил и реализовал задачу о эпидемии с помощью Julia и в OpenModelica.
