|test| |codecov| |docs|

.. |test| image:: https://github.com/intsystems/ProjectTemplate/workflows/test/badge.svg
    :target: https://github.com/intsystems/ProjectTemplate/tree/master
    :alt: Test status
    
.. |codecov| image:: https://img.shields.io/codecov/c/github/intsystems/ProjectTemplate/master
    :target: https://app.codecov.io/gh/intsystems/ProjectTemplate
    :alt: Test coverage
    
.. |docs| image:: https://github.com/intsystems/ProjectTemplate/workflows/docs/badge.svg
    :target: https://intsystems.github.io/ProjectTemplate/
    :alt: Docs status


.. class:: center

    :Название исследуемой задачи: Исправление грамматических ошибок в домене низкоресурсных языков
    :Тип научной работы: НИР
    :Автор: Хабутдинов Ильдар Айратович
    :Научный руководитель: к.ф-м.н, Грабовой Андрей Валериевич 

Abstract
========

В данной работе представлены два исследования, посвящённые задаче исправления грамматических ошибок в текстах с использованием подхода Sequence Tagging. В первом исследовании описывается адаптация модели GECToR для русского языка. С учетом недостатка размеченных данных, для обучения модели был создан синтетический набор данных. Разработанная модель показала хорошие результаты на синтетических данных $F_{0.5}$ = 82.5, а также продемонстрировала способность к переносу знаний на тестовый набор данных RULEC без дополнительного обучения $F_{0.5}$ = 22.2.

Во втором исследовании предлагается полностью автоматизированный, не требующий разметки подход к решению задачи исправления грамматических ошибок. Метод основан на генерации данных с использованием алгоритма Левенштейна для исправления грамматических ошибок на уровне подслов с использованием правил: keep, append, replace и delete. Подход универсален для любого языка и не требует дополнительной разметки. Применение данного метода к оригинальной модели GECToR позволило достичь конкурентных результатов на английском языке: $F_{0.5}$ = 62.4 на CoNLL-2014 и $F_{0.5}$ = 61.9 на BEA-2019, при этом не потребовалось ни аннотирования данных, ни составления словаря грамматических правил.

Таким образом, совместное рассмотрение обоих исследований демонстрирует возможности применения и адаптации Sequence Tag-ging моделей как для языков с достаточным количеством размеченных данных, так и для языков, где количество таких данных ограничено.

Research publications
===============================
1. RuGECToR: Rule-Based Neural Network Model for Russian Language Grammatical Error Correction
2. Automatic Spelling Correction for Russian: Multiple Error Approach
