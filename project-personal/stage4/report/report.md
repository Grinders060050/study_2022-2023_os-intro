---
## Front matter
title: "Индивидуальный проект этап 4"
subtitle: "Операционые системы"
author: "Шуваев Сергей Александрович"

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

Научиться вести дневник и вносить поправки на своем персональном сайте о своем жизненном опыте и не только...

# Задание

Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:
1. eLibrary : https://elibrary.ru/;
2. Google Scholar : https://scholar.google.com/;
3. ORCID : https://orcid.org/;
4. Mendeley : https://www.mendeley.com/;
5. ResearchGate : https://www.researchgate.net/;
6. Academia.edu : https://www.academia.edu/;
7. arXiv : https://arxiv.org/;
8. github : https://github.com/.
- Сделать пост по прошедшей неделе.
- Добавить пост на тему по выбору:
- Оформление отчёта.
- Создание презентаций.
- Работа с библиографией.

# Теоретическое введение

Файлы для редактирования информации о себе лежат в папке content/authors/_index.md/ Здесь можно редактировать информацию об авторах на сайте, а конкретно свою. Также рядом лежит папка, где хранится аватар в дополнение о себе.
Посты создаются и редактируются в папке posts. Для каждого поста создаётся своя папка, в которой должен лежать файл _index.md, а также и изображения, доступные для данного поста.

# Выполнение лабораторной работы

![Так как я ранее был зарегистрирован на eLibrary ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/1.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на Google Scholar ,просто захожу на ресурс,копирую и правлю информацию в файле](image/2.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на ORCID  ,просто захожу на ресурс,копирую и правлю информацию в файле](image/3.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на Mendeley ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/4.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на ResearchGate  ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/5.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на Academia.edu ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/6.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на arXiv ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/7.png){#fig:001 width=70%}

![Так как я ранее был зарегистрирован на github ,просто захожу на ресурс,копирую и правлю информацию в файле.](image/8.png){#fig:001 width=70%}

# Выводы

Я научился добавлять данные к сайту, написанном с помощью Hugo. 
Научился добавлять и редактировать посты.
