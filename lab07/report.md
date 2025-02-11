---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Введение в работу с данными"
author: "Лебедева Ольга Андреевна"

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

Основной целью работы является специализированных пакетов Julia для обработки
данных.

# Задачи 

- Освоить специализированные пакеты Julia для обработки данных.
- Научиться применять методы кластеризации, регрессии и анализа данных с использованием Julia.
- Ознакомиться с работой с файлами данных в формате CSV и структурой DataFrame.

# Термины и условные обозначения

- DataFrame — структура данных, аналогичная таблицам в базах данных.
- Кластеризация — метод машинного обучения для группировки объектов на основе их характеристик.
- Линейная регрессия — метод для нахождения линейной зависимости между переменными.
- PCA (Principal Component Analysis) — метод снижения размерности данных.
- k-средние — алгоритм кластеризации данных на основе центроидов.

# Объект и предмет исследования

Объект исследования: данные о недвижимости, включая цену, площадь, географическое расположение, а также данные о языках программирования.

Предмет исследования: применение алгоритмов обработки данных для анализа и визуализации.

# Техническое оснащение

Программное обеспечение: Jupyter Notebook, язык программирования Julia с установленными библиотеками (CSV, DataFrames, Clustering, Plots и др.).

Методы:
1. Считывание данных из файлов CSV.
Кластеризация данных методами k-средних и k ближайших соседей.
2. Применение PCA для снижения размерности.
3. Линейная регрессия для выявления зависимостей между переменными.

# Теоретическое введение

Обработка и анализ данных, полученных в результате проведения исследований, —
важная и неотъемлемая часть исследовательской деятельности. Большое значение имеет
выявление определённых связей и закономерностей в имеющихся неструктурированных
данных, особенно в данных больших размерностей. Выявленные в данных связей и закономерностей позволяет строить прогнозные модели с предполагаемым результатом. Для
решения таких задач применяют методы из таких областей знаний как математическая
статистика, программирование, искусственный интеллект, машинное обучение.

# Задание лабораторной работы №7

1. Используя Jupyter Lab, повторите примеры из раздела 7.2.
2. Выполните задания для самостоятельной работы (раздел 7.4).

Задание Cм. [рис. 1](#fig:001), Cм. [рис. 2](#fig:002)

![Задание_1](0_1.png){ #fig:001 width=70% }

![Задание_2](0_2.png){ #fig:002 width=70% }

# Выполнение лабораторной работы. Повторение примеров

Ниже приведены повторы примеров, данные в лабораторной работе для ознакомления: Cм. [рис. 3](#fig:003), Cм. [рис. 4](#fig:004), Cм. [рис. 5](#fig:005), Cм. [рис. 6](#fig:006), Cм. [рис. 7](#fig:007), Cм. [рис. 8](#fig:008), Cм. [рис. 9](#fig:009), Cм. [рис. 10](#fig:010),  Cм. [рис. 11](#fig:011), Cм. [рис. 12](#fig:012), Cм. [рис. 13](#fig:013), Cм. [рис. 14](#fig:014), Cм. [рис. 15](#fig:015), Cм. [рис. 16](#fig:016), Cм. [рис. 17](#fig:017), Cм. [рис. 18](#fig:018), Cм. [рис. 19](#fig:019), Cм. [рис. 20](#fig:020), Cм. [рис. 21](#fig:021).

![Повторение примеров_1)](1.png){#fig:003 width=75%}

![Повторение примеров_2](2.png){#fig:004 width=75%}

![Повторение примеров_3](3.png){#fig:005 width=75%}

![Повторение примеров_4](4.png){#fig:006 width=75%}

![Повторение примеров_5](5.png){#fig:007 width=75%}

![Повторение примеров_6](6.png){#fig:008 width=75%}

![Повторение примеров_7](7.png){#fig:009 width=75%}

![Повторение примеров_8](8.png){#fig:010 width=75%}

![Повторение примеров_9](9.png){#fig:011 width=75%}

![Повторение примеров_10](10.png){#fig:012 width=75%}

![Повторение примеров_11](11.png){#fig:013 width=75%}

![Повторение примеров_12](12.png){#fig:014 width=75%}

![Повторение примеров_13](13.png){#fig:015 width=75%}

![Повторение примеров_14](14.png){#fig:016 width=75%}

![Повторение примеров_15](15.png){#fig:017 width=75%}

![Повторение примеров_16](16.png){#fig:018 width=75%}

![Повторение примеров_17](17.png){#fig:019 width=75%}

![Повторение примеров_18](18.png){#fig:020 width=75%}

![Повторение примеров_19](19.png){#fig:021 width=75%}

# Самостоятельная работа

Выполним задание 7.4.1. Кластеризация: Cм. [рис. 22](#fig:022).

![Самостоятельная работа_1](20.png){#fig:022 width=75%}

Была выполнена кластеризация данных из набора iris с использованием языка Julia. Для этого данные были загружены с помощью библиотеки RDatasets, удалён столбец Species, а оставшиеся признаки преобразованы в матрицу и транспонированы для работы с алгоритмом k-средних.

С помощью библиотеки Clustering.jl данные были разделены на 10 кластеров. Результаты кластеризации визуализированы с использованием диаграммы рассеяния, где оси PetalLength и PetalWidth отражают размеры лепестков, а точки окрашены в зависимости от принадлежности к кластеру. В результате удалось продемонстрировать корректную работу алгоритма и его применение для анализа данных.

7.4.2. Регрессия (метод наименьших квадратов в случае линейной
регрессии). Cм. [рис. 23](#fig:023), Cм. [рис. 24](#fig:024), Cм. [рис. 25](#fig:025).

![Самостоятельная работа_2_1](21.png){#fig:023 width=75%}

![Самостоятельная работа_2_2](22.png){#fig:024 width=75%}

![Самостоятельная работа_2_3](23.png){#fig:025 width=75%}

Была выполнена линейная регрессия с использованием метода наименьших квадратов. Для этого были сгенерированы случайные данные и построена линейная зависимость между независимой переменной X и зависимой переменной y.

На графике представлена точечная диаграмма исходных данных (оранжевые точки) и линия регрессии (синяя линия), которая показывает оптимальное соответствие между переменными. Линия регрессии демонстрирует сильную положительную зависимость, что подтверждается коэффициентами регрессии, рассчитанными методом наименьших квадратов. Это визуализирует, как данный метод подходит для анализа линейных связей между переменными.

7.4.3. Модель ценообразования биномиальных опционов. Cм. [рис. 26](#fig:026), Cм. [рис. 27](#fig:027), Cм. [рис. 28](#fig:028).

В этом задании была реализована модель ценообразования биномиальных опционов. Первоначально была написана функция binomial_stock_price, которая рассчитывает траекторию изменения цены акций, используя параметры начальной цены, волатильности, процентной ставки и длины временного периода. Функция возвращает массив цен, где каждая последующая цена зависит от случайного события (рост или падение), что моделируется с помощью случайных чисел.

![Самостоятельная работа_3_1](24.png){#fig:026 width=75%}

На первом графике показана симуляция одной траектории изменения цены акции. Ось X представляет временные интервалы, а ось Y — стоимость акций. График демонстрирует динамику изменения цены, включая периоды роста и падения.

![Самостоятельная работа_3_2](25.png){#fig:027 width=75%}

Далее была реализована функция createPath, позволяющая сгенерировать несколько траекторий изменения цен. Результаты были визуализированы на втором графике, где представлены 10 различных траекторий. Каждая линия на графике — это отдельная симуляция изменения стоимости акции, что демонстрирует вариативность и влияние случайности на прогноз.

![Самостоятельная работа_3_3](26.png){#fig:028 width=75%}

Для оптимизации вычислений была использована параллельная обработка с помощью @threads, что позволило ускорить генерацию траекторий. На третьем графике представлены те же 10 траекторий, но они были сгенерированы с использованием многопоточности, что эффективно сокращает время расчётов при большом количестве симуляций.

Все графики отражают реалистичное поведение цен акций на рынке в условиях случайных изменений, что делает метод полезным для анализа и прогнозирования финансовых данных.

# Полученные результаты

1. Считаны и обработаны данные в формате CSV.
2. Реализованы алгоритмы кластеризации методом k-средних и анализа методом главных компонент (PCA).
3. Построены графики для визуализации результатов анализа данных.
4. Выполнен анализ линейной регрессии с использованием больших наборов данных.
5. Полученные результаты подтвердили эффективность использования Julia для обработки и анализа данных.

# Вывод

Научились работатать со специализированными пакетами Julia для обработки данных.

# Список литературы

[1] Julia: https://ru.wikipedia.org/wiki/Julia
