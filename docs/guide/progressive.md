---
sidebar_position: 2
---

# Как работает прогрессивная шкала

:::tip

Здесь описыается как работает прогрессивная шкала, а не как реально считать нало. Реальная шкала состоит из 2х частей — федеральной и региональной (кроме страны Басков и  Наварры), которые надо посчитать отдельно и потом сложить.

:::

Для просты пример возмем базовую шкалу, которую можно встретить на сайтах:

| Налоговая база (евро) | Налог от предыдущего брекета (евро) | Сумма брекета (евро) | Ставка налога (%) |
| --------------------- | ----------------------------------- | -------------------- | ----------------- |
| 0                     | 0                                   | 12450                | 19%               |
| 12450                 | 2365.50                             | 7750                 | 24%               |
| 20200                 | 4225.50                             | 15000                | 30%               |
| 35200                 | 8725.50                             | 24800                | 37%               |
| 60000                 | 17901.50                            | 240,000              | 45%               |
| 300000                | 125901.50                           | Remainder            | 47%               |

Многие читают табличку так — раз у меня доход 100000 евро в год, значит я попадаю в брекет 60000+ и буду платить 45%, но это не так. 

Правильный расчет будет выглядеть так:

1. Берем доход от 0 до 12450, на эту сумму будет налог 19%.
2. На доход от 12450 и 20200 будет 24%.
3. И так далее разбиваем ваш доход на брекеты.

Чтобы стало понятнее переделаем таблицу так:

| Начало брекета | Конец брекета | Сумма брекета | Ставка налога | Налог с брекета | Суммарный налог |
| -------------- | ------------- | ------------- | ------------- | --------------- | --------------- |
| 0              | 12450         | 12450         | 19%           | 2365.50         | 2365.50         |
| 12450          | 20200         | 7750          | 24%           | 1860            | 4225.50         |
| 20200          | 35200         | 15000         | 30%           | 4500            | 8725.50         |
| 35,200         | 60000         | 24800         | 37%           | 9176            | 17901.50        |
| 60,000         | 300000        | 240000        | 45%           | 108000          | 125901.50       |
| 300,000        |               |               | 47%           |                 |                 |

Теперь чтобы расчитать налог для дохода 100000 евро:

1. Находим брекет куда попадаешь наш налог — от 60000 до 300000. 
2. Смотрим сколько мы дожны налогов от нижних брекетов — 17,901.50.
3. Считаем остаток `(100000-60000)*37%=14800`
4. Считаем финальный налог `14800+17901.50=32701.50`
5. Считаем эффективную ставку `32701.50/100000=32.7%` 

Получилось, что ваш налог не 45%, а 32,7%.