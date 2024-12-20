---
## Front matter
lang: ru-RU
title: "Лабораторная работа №4. Линейная алгебра" 
subtitle: 
author: |
        Выполнила: Лебедева Ольга Андреевна
institute: |
           Российский университет дружбы народов, Москва, Россия
date: |
      2024

babel-lang: russian
babel-otherlangs: english
mainfont: Arial
monofont: Courier New
fontsize: 8pt

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

## Цель работы

Основной целью работы является изучение возможностей специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной
алгебры.

## Задачи

- Изучение возможностей языка программирования Julia для выполнения операций линейной алгебры.
Закрепление навыков работы с векторами и матрицами
- Решение систем линейных уравнений.
- Приведение матриц к диагональному виду.
- Вычисление собственных значений и векторов матриц.
- Оценка эффективности выполнения операций с использованием встроенных библиотек.

## Объект и предмет исследования

Объектом исследования являются векторы и матрицы, их математические свойства и операции с ними.

Исследуются также программные средства (функции языка Julia) для работы с линейной алгеброй.

## Условные обозначения и термины

Вектор — одномерный массив чисел, представляющий величины с направлением.

Матрица — двумерный массив чисел, используемый для представления систем уравнений или линейных преобразований.

Скалярное произведение — сумма произведений соответствующих элементов двух векторов.

Внешнее произведение — операция, создающая матрицу из двух векторов.

Продуктивность матрицы — свойство, определяющее возможность решения линейной модели (E−A)x=y с неотрицательными значениями.

## Техническое оснащение и выбранные методы проведения работы

Основные вычисления реализованы в среде Jupyter Notebook с применением библиотеки LinearAlgebra для операций с матрицами, спектрального разложения и решения СЛАУ.

## Теоретическое введение

Julia — высокоуровневый свободный язык программирования с динамической типизацией, созданный для математических вычислений. Эффективен также и для написания программ общего назначения[1].

## Задание

1. Используя Jupyter Lab, повторите примеры из раздела 4.2.
2. Выполните задания для самостоятельной работы (раздел 4.4).

## Выполнение лабораторной работы. Самостоятельное выполнение

Задание Cм. [рис. 1](#fig:001), Cм. [рис. 2](#fig:002), Cм. [рис. 3](#fig:003)

![Задание_1](24.png){ #fig:001 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

![Задание_2](25.png){ #fig:002 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

![Задание_3](26.png){ #fig:003 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 1: Cм. [рис. 4](#fig:004)

![Задание 1_1](1.png){ #fig:004 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

Для выполнения задания был задан вектор 
𝑣=[1,2,3]. Затем с помощью функции dot было вычислено скалярное произведение, а матричное произведение было получено умножением вектора 𝑣 его транспонированный вариант 𝑣′.

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 2: Cм. [рис. 5](#fig:004), Cм. [рис. 6](#fig:006)

![Задание 2_1](2.png){ #fig:005 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

![Задание 2_2](3.png){ #fig:006 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

Системы могут быть:
- Совместными (имеющими одно или несколько решений).
- Несовместными (не имеющими решений).

Для решения СЛАУ использовался оператор обратного слэша \, который автоматически выбирает оптимальный метод для нахождения решения.

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 3.1-3.2: Cм. [рис. 7](#fig:007), Cм. [рис. 8](#fig:008)

![Задание 3_1](4.png){ #fig:007 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

![Задание 3_2](5.png){ #fig:008 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

- Приведение к диагональному виду выполнялось через спектральное разложение: были найдены собственные значения и собственные векторы матрицы.
- Собственные значения формируют диагональную матрицу, а собственные векторы — матрицу преобразования.

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 3.2: Cм. [рис. 9](#fig:009)

![Задание 3.2](6.png){ #fig:009 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

- Возведение в степень или извлечение корня реализовывалось через спектральное разложение, что позволило работать с матрицами, включая те, которые имеют отрицательные собственные значения.
- Спектральный метод позволяет вычислять дробные степени матрицы, если преобразовать собственные значения в комплексный тип.

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 3.3: Cм. [рис. 10](#fig:010), 

![Задание 3.3](7.png){ #fig:010 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

- Были найдены собственные значения заданной матрицы, на основе которых была сформирована диагональная матрица.
- Также была создана нижнетреугольная матрица с элементами исходной матрицы.

## Выполнение лабораторной работы. Самостоятельное выполнение

Выполним задание 4: Cм. [рис. 11](#fig:011), Cм. [рис. 12](#fig:012)

![Заданиe 4](8.png){ #fig:011 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

![Задание 4_1](9.png){ #fig:012 width=70% }

## Выполнение лабораторной работы. Самостоятельное выполнение

Линейная модель экономики реализовывалась через проверку продуктивности матриц.

Было проверено три критерия:
- Возможность решения системы.
- Наличие обратной матрицы (E−A)^−1.
- Спектральный критерий (все собственные значения по модулю меньше 1).

## Полученные результаты

1. Лабораторная работа позволила изучить базовые операции линейной алгебры, такие как умножение векторов, работа с матрицами, спектральное разложение и решение систем уравнений.

2. Реализация на Julia показала эффективность использования встроенных функций и библиотек для работы с линейной алгеброй.

## Заключение

Изучили возможности специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной алгебры.

## Библиографическая справка 

[1] Julia: https://ru.wikipedia.org/wiki/Julia

