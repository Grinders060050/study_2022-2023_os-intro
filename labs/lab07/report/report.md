---
## Front matter
title: "Отчет по лабораторной работе №7"
subtitle: "Операционные системы"
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

Цель данной лабораторной работы - освоение основных возможностей командной оболочки Midnight Commander, приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними

# Задание

## Задание по mc

1. Изучите информацию о mc, вызвав в командной строке man mc.
2. Запустите из командной строки mc, изучите его структуру и меню.
3. Выполните несколько операций в mc, используя управляющие клавиши (операции с панелями; выделение/отмена выделения файлов, копирование/перемещение файлов, получение информации о размере и правах доступа на файлы и/или каталоги и т.п.)
4. Выполните основные команды меню левой (или правой) панели. Оцените степень подробности вывода информации о файлах.
5. Используя возможности подменю Файл , выполните:
6. просмотр содержимого текстового файла;
7. редактирование содержимого текстового файла (без сохранения результатов редактирования);
8. создание каталога;
9. копирование в файлов в созданный каталог.
10. С помощью соответствующих средств подменю Команда осуществите:
11. поиск в файловой системе файла с заданными условиями (например, файла с расширением .c или .cpp, содержащего строку main);
12. выбор и повторение одной из предыдущих команд;
13. переход в домашний каталог;
14. анализ файла меню и файла расширений.
15. Вызовите подменю Настройки . Освойте операции, определяющие структуру экрана mc (Full screen, Double Width, Show Hidden Files и т.д.)

##Задание по встроенному редактору mc

Создайте текстовой файл text.txt.
Откройте этот файл с помощью встроенного в mc редактора.
Вставьте в открытый файл небольшой фрагмент текста, скопированный из любого другого файла или Интернета.
Проделайте с текстом следующие манипуляции, используя горячие клавиши:
Удалите строку текста.
Выделите фрагмент текста и скопируйте его на новую строку
Выделите фрагмент текста и перенесите его на новую строку.
Сохраните файл.
Отмените последнее действие.
Перейдите в конец файла (нажав комбинацию клавиш) и напишите некоторый текст.
Перейдите в начало файла (нажав комбинацию клавиш) и напишите некоторый текст. 4.8. Сохраните и закройте файл.
Откройте файл с исходным текстом на некотором языке программирования (напри- мер C или Java)
Используя меню редактора, включите подсветку синтаксиса, если она не включена, или выключите, если она включена
Теоретическое введение
Командная оболочка — интерфейс взаимодействия пользователя с операционной системой и программным обеспечением посредством команд. Midnight Commander (или mc) — псевдографическая командная оболочка для UNIX/Linux систем. Для запуска mc необходимо в командной строке набрать mc и нажать Enter .

MC имеет много полезных как для пользователей, так и для администраторов, функций (копирование, удаление, переименование/перемещение, создание директорий).

Главное окно программы Midnight Commander состоит из трех полей. Два поля, называемые "панелями", идентичны по структуре и обычно отображают перечни файлов и подкаталогов каких-то двух каталогов файловой структуры. Эти каталоги в общем случае различны, хотя, в частности, могут и совпасть. Каждая панель состоит из заголовка, списка файлов и информационной строки.

Третье поле экрана, расположенное в нижней части экрана, содержит командную строку текущей оболочки. В этом же поле (самая нижняя строка экрана) содержится подсказка по использованию функциональных клавиш F1 - F10. Самая верхняя строка экрана содержит строку горизонтального меню. Эта строка может не отображаться на экране; в этом случае доступ к ней можно получить, щёлкнув мышью по верхней рамке или нажав клавишу F9.

# Теоретическое введение

Командная оболочка — интерфейс взаимодействия пользователя с операционной системой и программным обеспечением посредством команд. Midnight Commander (или mc) — псевдографическая командная оболочка для UNIX/Linux систем. Для запуска mc необходимо в командной строке набрать mc и нажать Enter .

MC имеет много полезных как для пользователей, так и для администраторов, функций (копирование, удаление, переименование/перемещение, создание директорий).

Главное окно программы Midnight Commander состоит из трех полей. Два поля, называемые "панелями", идентичны по структуре и обычно отображают перечни файлов и подкаталогов каких-то двух каталогов файловой структуры. Эти каталоги в общем случае различны, хотя, в частности, могут и совпасть. Каждая панель состоит из заголовка, списка файлов и информационной строки.

Третье поле экрана, расположенное в нижней части экрана, содержит командную строку текущей оболочки. В этом же поле (самая нижняя строка экрана) содержится подсказка по использованию функциональных клавиш F1 - F10. Самая верхняя строка экрана содержит строку горизонтального меню. Эта строка может не отображаться на экране; в этом случае доступ к ней можно получить, щёлкнув мышью по верхней рамке или нажав клавишу F9.

# Выполнение лабораторной работы

![С помощью команды man mc прочитал документацию про командную оболочку](image/1.png){#fig:001 width=70%}

![Ввожу в терминале mc и получаю окно, в котором далее смогу работать ](image/2.png){#fig:001 width=70%}

![ помощью стрелочек влево вправо я могу перемещаться по директориям, а с помощью стрелочек вверх вниз перебирать файлы в директории, в которой нахожусь ](image/3.png){#fig:001 width=70%}

![С помощью F5 могу создать копию файла в выбранном каталоге](image/4.png){#fig:001 width=70%}

![С помощью управляющих клавиш так же можно получить информациб о правах доступа на файл и информацию о нем](image/5.png){#fig:001 width=70%}

![В меню правой панели вывел информацию о файле, получаю информации больше чем в выводе ls -l ](image/6.png){#fig:001 width=70%}

![Используя возможности подменю "Файл" я просмотрела содержимое текстового файла](image/7.png){#fig:001 width=70%}

![Открыл файл на изменение, поменял пару строк и закрыла файл без сохранения ](image/8.png){#fig:001 width=70%}

![Создаю каталог family ](image/9.png){#fig:001 width=70%}

![Копирую файл в созданный каталог (рис. @fig:010). Действия выше можно было сделать с помощью горячих клавиш. ](image/10.png){#fig:001 width=70%}

![С помощью средств подменю Команда можно найти файл с заданным условием, я искал файлы формата .txt ](image/11.png){#fig:001 width=70%}

![Можно перемещаться между директориями, я перемещусь в домашнюю](image/12.png){#fig:001 width=70%}

![Можно использовать историю команд и применить команду из истории, я применил копирование файла](image/12.png){#fig:001 width=70%}

![Анализирую файл меню](image/13.png){#fig:001 width=70%}

![Из подменю настройки вызвал окна настройки панели (рис. @fig:016), настройки внешнего вида (рис. @fig:017), настройки распознавания клавиш (рис. @fig:018), параметры конфигурации (рис. @fig:019).](image/14.png){#fig:001 width=70%}

![](image/15.png){#fig:001 width=70%}

![](image/16.png){#fig:001 width=70%}

![](image/17.png){#fig:001 width=70%}

![](image/18.png){#fig:001 width=70%}

![](image/19.png){#fig:001 width=70%}

![](image/20.png){#fig:001 width=70%}

![Командой touch text.txt создал файл](image/21.png){#fig:001 width=70%}

![Клавишей F4 открыл файл для записи, добавил в него текст](image/22.png){#fig:001 width=70%}

![Выделяю текст с помощью клавиши F3 и кликов мышью ](image/23.png){#fig:001 width=70%}

![Удалил строку текста с помощью ctrl+y (](image/24.png){#fig:001 width=70%}

![Сохраняю изменения в файле с помощью горячей клавиши F2](image/25.png){#fig:001 width=70%}

![С помощью ctrl+u отменяю последнее действие и возвращаю удаленную строку](image/26.png){#fig:001 width=70%}

![С помощью клавиш pgup pgdn у меня получилось попасть в начало и в конец файла соответственно, я добавил текст в начало и в конец файла ](image/27.png){#fig:001 width=70%}

![Горячая клавиша F10 закрывает файл, дополнительно спрашивая сохранить ли в нем несохраненные изменения, сохраняю и закрываю (](image/28.png){#fig:001 width=70%}

![Открываю файл формата .cpp, с кодом на С++, встроенный редактор mc вывел его содержимое с подсветкой ](image/29.png){#fig:001 width=70%}

![Я отключил подсветку и вывел снова тот же самый файл, но уже без подсветки](image/30.png){#fig:001 width=70%}

# Выводы

При выполнениии данной лабораторной работы я освоил основные возможности командной оболочки Midnight Commander, приобрел навыки практической работы по просмотру каталогов и файлов; манипуляций с ними

# Ответы на контрольные вопросы

Какие режимы работы есть в mc. Охарактеризуйте их. Панели могут дополнительно быть переведены в один из двух режимов: Информация или Дерево. В режиме Информация на панель выводятся сведения о файле и текущей файловой системе, расположенных на активной панели. В режиме Дерево (рис. 7.3) на одной из панелей выводится структура дерева каталогов.

Какие операции с файлами можно выполнить как с помощью команд shell, так и с помощью меню (комбинаций клавиш) mc? Приведите несколько примеров. В разделе Командная строка оболочки (Shell) перечисляются команды и комбинации клавиш, которые используются для ввода и редактирования команд в командной строке оболочки. Большая часть этих команд служит для переноса имен файлов и/или имен каталогов в командную строку (чтобы уменьшить трудоемкость ввода) или для доступа к истории команд. Клавиши редактирования строк ввода используются как при редактировании командной строки, так и других строк ввода, появляющихся в различных запросах программы.

Как с помощью меню так и с помощью команд shell можно переносить, копировать и получать информацию о файоах и каталогах.

Опишите структура меню левой (или правой) панели mc, дайте характеристику командам.
В меню каждой (левой или правой) панели можно выбрать Формат списка:

стандартный — выводит список файлов и каталогов с указанием размера и времени правки;
ускоренный — позволяет задать число столбцов, на которые разбивается панель при выводе списка имён файлов или каталогов без дополнительной информации;
расширенный — помимо названия файла или каталога выводит сведения о правах доступа, владельце, группе, размере, времени правки;
определённый пользователем — позволяет вывести те сведения о файле или каталоге, которые задаст сам пользователь.
Опишите структура меню Файл mc, дайте характеристику командам. В меню Файл содержит перечень команд, которые могут быть применены к одному или нескольким файлам или каталогам.
Команды меню Файл:

Просмотр ( F3 ) — позволяет посмотреть содержимое текущего (или выделенного) файла без возможности редактирования.
Просмотр вывода команды ( М + ! ) — функция запроса команды с параметрами (аргумент к текущему выбранному файлу).
Правка ( F4 ) — открывает текущий (или выделенный) файл для его редактирования.
Копирование ( F5 ) — осуществляет копирование одного или нескольких файлов или каталогов в указанное пользователем во всплывающем окне место.
Права доступа ( Ctrl-x c ) — позволяет указать (изменить) права доступа к одному или нескольким файлам или каталогам .
Жёсткая ссылка ( Ctrl-x l ) — позволяет создать жёсткую ссылку к текущему (или выделенному) файлу.
Символическая ссылка ( Ctrl-x s ) — позволяет создать символическую ссылку к текущему (или выделенному) файлу.
Владелец/группа ( Ctrl-x o ) — позволяет задать (изменить) владельца и имя группы для одного или нескольких файлов или каталогов.
Права (расширенные) — позволяет изменить права доступа и владения для одного или нескольких файлов или каталогов.
Переименование ( F6 ) — позволяет переименовать (или переместить) один или несколько файлов или каталогов.
Создание каталога ( F7 ) — позволяет создать каталог.
Удалить ( F8 ) — позволяет удалить один или несколько файлов или каталогов.
Выход ( F10 ) — завершает работу mc.
Опишите структура меню Команда mc, дайте характеристику командам.
В меню Команда содержатся более общие команды для работы с mc. Команды меню Команда:

Дерево каталогов — отображает структуру каталогов системы.
Поиск файла — выполняет поиск файлов по заданным параметрам.
Переставить панели — меняет местами левую и правую панели.
Сравнить каталоги ( Ctrl-x d ) — сравнивает содержимое двух каталогов.
Размеры каталогов — отображает размер и время изменения каталога (по умолчанию в mc размер - каталога корректно не отображается).
История командной строки — выводит на экран список ранее выполненных в оболочке команд.
Каталоги быстрого доступа ( Ctrl-\ ) — пр вызове выполняется быстрая смена текущего каталога на один из заданного списка.
Восстановление файлов — позволяет восстановить файлы на файловых системах ext2 и ext3.
Редактировать файл расширений — позволяет задать с помощью определённого синтаксиса действия при запуске файлов с определённым расширением (например, какое программного обеспечение запускать для открытия или редактирования файлов с расширением doc или docx).
Редактировать файл меню — позволяет отредактировать контекстное меню пользователя, вызываемое по клавише F2 .
Редактировать файл расцветки имён — позволяет подобрать оптимальную для пользователя расцветку имён файлов в зависимости от их типа.
Опишите структура меню Настройки mc, дайте характеристику командам.
Меню Настройки содержит ряд дополнительных опций по внешнему виду и функциональности mc. Меню Настройки содержит:

Конфигурация — позволяет скорректировать настройки работы с панелями.
Внешний вид и Настройки панелей — определяет элементы (строка меню, командная строка, подсказки и прочее), отображаемые при вызове mc, а также геометрию расположения панелей и цветовыделение.
Биты символов — задаёт формат обработки информации локальным терминалом.
Подтверждение — позволяет установить или убрать вывод окна с запросом подтверждения действий при операциях удаления и перезаписи файлов, а также при выходе из программы.
Распознание клавиш — диалоговое окно используется для тестирования функциональных клавиш, клавиш управления курсором и прочее.
Виртуальные ФС –– настройки виртуальной файловой системы: тайм-аут, пароль и прочее.
Назовите и дайте характеристику встроенным командам mc.

F1 Вызов контекстно-зависимой подсказки;
F2 Вызов пользовательского меню с возможностью создания и/или дополнения дополнительных функций;
F3 Просмотр содержимого файла, на который указывает подсветка в активной панели (без возможности редактирования);
F4 Вызов встроенного в mc редактора для изменения содержания файла, на который указывает подсветка в активной панели;
F5 Копирование одного или нескольких файлов, отмеченных в первой (активной) панели, в каталог, отображаемый на второй панели;
F6 Перенос одного или нескольких файлов, отмеченных в первой (активной) панели, в каталог, отображаемый на второй панели;
F7 Создание подкаталога в каталоге, отображаемом в активной панели;
F8 Удаление одного или нескольких файлов (каталогов), отмеченных в первой (активной) панели файлов;
F9 Вызов меню mc;
F10 Выход из mc;
Назовите и дайте характеристику командам встроенного редактора mc.

Ctrl-y удалить строку;
Ctrl-u отмена последней операции; Ins вставка/замена;
F7 поиск (можно использовать регулярные выражения);
(стрелочка вверх)-F7 повтор последней операции поиска;
F4 замена;
F3 первое нажатие — начало выделения,
второе — окончание выделения;
F5 копировать выделенный фрагмент;
F6 переместить выделенный фрагмент;
F8 удалить выделенный фрагмент;
F2 записать изменения в файл;
F10 выйти из редактора.
Дайте характеристику средствам mc, которые позволяют создавать меню, определяемые пользователем.

Можете сохранить часто используемые команды панелизации под отдельными информативными именами, чтобы иметь возможность их быстро вызвать по этим именам. Для этого нужно набрать команду в строке ввода (строка "Команда") и нажать кнопку Добавить. После этого потребуется ввести имя, по которому мы будем вызывать команду. В следующий раз вам достаточно будет выбрать нужное имя из списка, а не вводить всю команду заново.

Дайте характеристику средствам mc, которые позволяют выполнять действия, определяемые пользователем, над текущим файлом.
Панель в mc отображает список файлов текущего каталога. Абсолютный путь к этому каталогу отображается в заголовке панели. У активной панели заголовок и одна из её строк подсвечиваются. Управление панелями осуществляется с помощью определённых комбинаций клавиш или пунктов меню mc.

::: {#refs}
:::
