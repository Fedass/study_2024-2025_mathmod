---
## Front matter
title: "Этап 1"
subtitle: "Научная проблема проекта Рост дендритов"
author: 

  - Городянский Ф.Н.
  - Дзахмишев К.З.

# Generic otions
lang: ru-RU
toc-title: "Содержание"

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


# Введение

**Актуальность**

Дендриты представляют собой разветвлённые отростки нейронов, обеспечивающие передачу и обработку электрических и химических сигналов. Их развитие играет важную роль в функционировании нервной системы, влияя на когнитивные процессы, обучение и память. Дендритный рост является сложным биологическим процессом, зависящим от множества факторов, таких как генетика, внешние сигналы и внутренняя активность нейронов. Нарушения в развитии дендритов могут приводить к различным неврологическим и психиатрическим заболеваниям, таким как аутизм, шизофрения и нейродегенеративные расстройства. Поэтому изучение роста дендритов имеет как фундаментальное, так и прикладное значение.

**Цель работы**

Основной целью исследования является изучение механизмов роста дендритов, факторов, влияющих на их развитие, и возможных способов регулирования этих процессов. 


**Задачи**


- Рассмотреть биологические основы роста дендритов, включая молекулярные и клеточные механизмы.
- Исследовать влияние внешних и внутренних факторов, таких как нейротрофины, электрическая активность и механическая среда, на формирование дендритной структуры.
- Описать существующие математические и компьютерные модели, применяемые для изучения роста дендритов, и сравнить их с экспериментальными данными.
- Определить роль дендритного роста в когнитивных функциях, пластичности мозга и развитии нервной системы.
- Рассмотреть перспективы исследований в области регулирования дендритного роста для лечения неврологических заболеваний.

# Теоретическое описание задачи

**Биологические основы роста дендритов**

Рост дендритов регулируется сложными биохимическими механизмами. Основную роль играют:
- Нейротрофины – белки, способствующие росту и выживанию нейронов. Среди них наиболее изучены фактор роста нервов (NGF) и мозговой нейротрофический фактор (BDNF), которые активируют сигнальные пути, ведущие к развитию и ветвлению дендритов.
- Кальциевые сигналы – влияют на рост и реорганизацию дендритных ветвей. Колебания внутриклеточного уровня кальция регулируют полимеризацию актинового цитоскелета, который формирует структуру дендритов.
- Гены и белки – например, белок DSCAM играет ключевую роль в регуляции дендритной морфологии и предотвращает излишнюю ветвистость.
- Электрическая активность – синаптическая активность стимулирует или подавляет рост дендритов в зависимости от характера входных сигналов.

Влияние внешних факторов

Помимо внутренних механизмов, на рост дендритов влияет окружающая среда. Например, сенсорный опыт, обучение и стрессы могут изменять структуру дендритов. В опытах на животных показано, что обогащённая среда (наличие стимулов, таких как игрушки и лабиринты) способствует увеличению числа дендритных ветвей, тогда как социальная изоляция подавляет их развитие. Дефицит питательных веществ, таких как омега-3 жирные кислоты, также может негативно сказаться на дендритном росте.

**Описание моделей роста дендритов**

Моделирование роста дендритов включает несколько подходов:
1. Стохастические модели – основаны на вероятностных законах ветвления и роста. Они учитывают случайные процессы формирования новых ответвлений и конкуренцию за ресурсы.
2. Динамические модели на основе уравнений – описывают рост с использованием дифференциальных уравнений, отражающих влияние биохимических факторов.
3. Клеточные автоматы – модели, основанные на локальных правилах взаимодействия между клеточными элементами, имитирующие морфогенез нейронов.
4. Компьютерные симуляции – используют алгоритмы, приближённые к реальной нейронной сети, чтобы анализировать, как разные параметры влияют на морфологию дендритов.

Модели помогают понять, как внешние стимулы и биохимические процессы влияют на формирование дендритной структуры. Например, компьютерные симуляции показывают, что увеличение концентрации BDNF приводит к усиленному росту дендритов, что подтверждается и экспериментальными данными.

**Значение дендритного роста для нервной системы**

Рост и организация дендритов определяют эффективность нейронных связей, что критично для когнитивных процессов, памяти и адаптации к изменяющимся условиям. Дендритная пластичность играет ключевую роль в обучении: усиление связей между активно используемыми синапсами ведёт к структурным изменениям дендритного дерева.

Нарушения в росте дендритов ассоциируются со многими заболеваниями. Например:
- При болезни Альцгеймера наблюдается дегенерация дендритов, приводящая к когнитивному снижению.
- Шизофрения связана с уменьшением количества дендритных шипиков, что ухудшает синаптическую передачу.
- В аутистическом спектре наблюдаются как избыточное ветвление дендритов, так и нарушения их структуры.

Исследования роста дендритов могут помочь в разработке методов лечения этих заболеваний, например, с использованием нейротрофинов или электрической стимуляции.


# Выводы

Во время выполнения первого этапа группового проекта мы сделали теоретическое описание моделей роста дендритов и определили задачи дальнейшего исследования.

# Список литературы{.unnumbered}

::: {#refs}
:::