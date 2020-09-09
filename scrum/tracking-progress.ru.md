---
title: Отслеживание Прогресса в Спринте
order: 700
---

Команда в Scrum самоуправляема, и для того, чтобы делать это успешно, она должна знать, как это происходит. Каждый день члены Команды обновляют свою оценку оставшейся до завершения работы в **Бэклоге Спринта** (Иллюстрация 6). Обычно также кто-то суммирует всю оставшуюся работу для Команды в целом, и отмечает её **Диаграмму Сгорания Спринта** (Sprint Burndown Chart) (Иллюстрации 7 и 8). На этом графике каждый день отображается новая оценка того, сколько Команде осталось работы в этом Спринте. В идеале, это наклонный *нисходящий* график, который находится на траектории достижения “нулевого остатка работы” к последнему дню Спринта. И хотя иногда это выглядит хорошо, часто это не так; это реальность продуктовой разработки. Важно то, что он показывает Команде их *прогресс* в достижении цели не с точки зрения того, сколько времени было потрачено в прошлом (несущественный факт с точки зрения прогресса), а с точки зрения того, сколько работы *осталось в будущем* - то, что отделяет Команду от её цели. Если линия на Диаграмме Сгорания не стремится вниз ближе к завершению Спринта, тогда Команде необходимо адаптироваться, например, чтобы уменьшить объём работы или найти способ работать более эффективно, сохраняя при этом устойчивый темп.

Хотя Диаграмму Сгорания Спринта можно создать и отобразить с помощью электронных таблиц, многие команды считают более эффективным отображать её на бумаге, на стене своей рабочей комнаты, обновляя её шариковой ручкой; это “низко технологичное/высоко ощущаемое” (low-tech/high-touch) решение работает быстро, просто и часто более наглядно, чем компьютерная диаграмма.

<table class="grid_table_with_header">
  <thead>
    <tr>
      <th style="text-align: center">Элемент Бэклога Продукта</th>
      <th style="text-align: center">Задача</th>
      <th style="text-align: center">Волонтёр</th>
      <th style="text-align: center">Первоначальная оценка</th>
      <th colspan="6" style="text-align: center">New Estimates of Effort remaining at end of day...</th>
    </tr>
    <tr>
      <th></th><th></th><th></th><th></th>
      <th style="text-align: center">1</th>
      <th style="text-align: center">2</th>
      <th style="text-align: center">3</th>
      <th style="text-align: center">4</th>
      <th style="text-align: center">5</th>
      <th style="text-align: center">6</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Как покупатель, Я хочу положить книгу в корзину</td>
      <td>Изменить БД</td>
      <td>Санджей</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">4</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">0</td>
      <td style="text-align: center">0</td>
      <td style="text-align: center">0</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Создать страницу (UI)</td>
      <td>Джинг</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">2</td>
      <td style="text-align: center">0</td>
      <td style="text-align: center">0</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Создать страницу (JavaScript)</td>
      <td>Трейси и Сэм</td>
      <td style="text-align: center">2</td>
      <td style="text-align: center">2</td>
      <td style="text-align: center">2</td>
      <td style="text-align: center">1</td>
      <td style="text-align: center">0</td>
      <td style="text-align: center">0</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Написать автоматические приёмочные тесты</td>
      <td>Sarah</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">0</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Обновить раздел помощи для покупателей</td>
      <td>Санджей and Джинг</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">0</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>...</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>Улучшить производительность обработки транзакций</td>
      <td>Объединить DCP код и законченные тесты слоёв</td>
      <td></td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Закончить машинный заказ для pRank</td>
      <td></td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">3</td>
      <td style="text-align: center">8</td>
      <td style="text-align: center">8</td>
      <td style="text-align: center">8</td>
      <td style="text-align: center">8</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Изменить DCP и читателя для использования pRank в  HTTP API</td>
      <td></td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td style="text-align: center">5</td>
      <td></td>
    </tr>
  </tbody>
</table>

**Иллюстрация 6.** Ежедневное Обновление Оставшейся Работы в Бэклоге Спринта
{: .table-figure-caption}


<div>
  {% figure "img/scrum/sprint-burndown", "Иллюстрация 7. Диаграмма Сгорания Спринта", class:"two-third-sized-figure", caption: true %}
</div>

<div>
  {% figure "img/scrum/hand-drawn-sprint-burndown", "Иллюстрация 8. Визуальное Управления: Нарисованная от руки Диаграмма Сгорания Спринта", class:"two-third-sized-figure", caption: true %}
</div>

Перевод статьи осуществлён [Кротовым Артёмом](https://www.facebook.com/artem.v.krotov) и [Романом Лапаевым](https://www.linkedin.com/in/romanlapaev).
