# Определение драйверов изменения цены лечения медицинской клиники

## СФЕРА
- медицина

## СТЕК
- Python
- Pandas
- Nympy
- Plotly
- Seaborn
- Matplotlib
- Re

## ОПИСАНИЕ / КОНТЕКСТ ПРОЕКТА
В рамках проекта вы поработаете с реальными сырыми данными от одного медицинского центра.
Требуется оценить вклад различных факторов в изменение средней стоимости лечения в медицинской клинике в разные годы.
Проанализировать изменение выручки медицинского центра в 2022 году относительно 2021 и выявить ключевые факторы, повлиявшие на это изменение.

## ЦЕЛЬ
Провести анализ изменения цены лечения в медицинской клинике в 2022 году относительно 2021 года, определить ключевые драйверы изменения цены лечения.

## ВЫВОДЫ
Исследование показало, что в 2022 году стоимость одной услуги и стоимость лечения выросла.
Был провдён анализ изменений стоимости услуг, в ходе которого удалось определить, что у 66% услуг выросла цена (но у большинства - не более, чем на 25%). Основные изменения цены произошли после октября 2021 года - тогда же, судя по всему, часть услуг была переименована (например, первичные и повторные приёмы стали включать названия специалистов).
Самый популярный тип услуги, приём (входящий в большую часть визитов), также изменил свою стоимость.

В ходе анализа удалось определить, как изменился портрет клиента клиники в 2022 году относительно 2021:
- стало немного меньше детей и больше взрослых в возрасте от 18 до 44 лет,
- соотношение женщин и мужчин практически не изменилось (женщин, как и в 2021 году больше).

__ГИПОТЕЗЫ__

Было выдвинуто 3 гипотезы:
1. Изменение стоимости услуг оказывает незначительное влияние на изменение стоимости визита.
Гипотеза была подтерждена (корреляция Пирсона для заданых параметров составила 0.37)
2. Количество услуг визита влияет на общую стоимость визита.
Гипотеза была подтверждена (корреляция Пирсона - 0.79). Но так как медианное количество услуг для визитов в 2021 и 2022 году одинаковое, можно предположить, что количество услуг визита не является ключевым драйвером изменения стоимости лечения.
3. Изменение стоимости приёмов влияет на стоимость визита.
Гипотеза была подтерждена (корреляция Пирсона - 0.53). 71% визитов включают в себя разные виды приёмов. И так как медианная стоимость приёма в 2022 году выше, чем в 2021, можно предположить, что изменение стоимости приёмов является одним из ключевых драйверов изменения стоимости лечения в целом.


