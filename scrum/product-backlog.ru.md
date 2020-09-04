---
title: Бэклог Продукта
order: 300
---

При переходе продуктовой группы на Скрам перед стартом первого Спринта им необходим **Бэклог Продукта** (Product Backlog), приоритизированный (упорядоченный 1, 2, 3, ...) список задач, ориентированных на клиента.  
Бэклог Продукта существует (и развивается) на протяжении всего жизненного цикла продукта; это дорожная карта (roadmap) продукта (**Иллюстрации 2 и 3**). В любой момент Бэклог Продукта является единственным, исчерпывающим представлением “всего, что могло быть бы сделано Командой когда-либо, в порядке приоритета”. Для продукта существует только единственный Бэклог Продукта; это означает, что Владелец Продукта необходим, чтобы принимать решения о приоритизации на всём спектре, предоставляя интересы заинтересованных лиц (включая Команду).

<table class="grid_table_with_header">
  <thead>
    <tr>
      <th style="text-align: center">Приоритет</th>
      <th style="text-align: center">Элемент</th>
      <th style="text-align: center">Делали (ссылка на Вики)</th>
      <th style="text-align: center">Первоначальная оценка</th>
      <th colspan="6" style="text-align: center">Оценка в Спринте</th>
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
      <td style="text-align: center">1</td>
      <td>Как покупатель, Я хочу положить книгу в корзину (см. наброски UI в вики)</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">5</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">2</td>
      <td>Как покупатель, Я хочу удалять книги из корзины</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">2</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">3</td>
      <td>Улучшить производительность процессинга транзакции (см. целевые метрики производительности в вики)</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">4</td>
      <td>Исследовать решение для ускорения проверки кредитной карты (см. целевые метрики производительности в вики)</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">20</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">5</td>
      <td>Обновить версию Apache до 2.2.3 на всех серверах</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">6</td>
      <td>Диагностировать и исправить ошибки порядка исполнения скриптов (bugzilla ID 14823)</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">3</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">7</td>
      <td>Как покупатель, Я хочу создавать и сохранять список желаний</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">40</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td style="text-align: center">8</td>
      <td>Как покупатель, Я хочу добавлять и удалять элементы м мой список желаний</td>
      <td style="text-align: center">…</td>
      <td style="text-align: center">20</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
  </tbody>
</table>

**Иллюстрация 2**. Бэклог Продукта
{: .table-figure-caption}

<div>
  {% figure "img/scrum/product-backlog-visual-management", "Иллюстрация 3. Визуальное Управление: Элементы Бэклог Продукта на стене", caption: true,  class:"half-sized-figure pull-right" %}
</div>

Бэклог Продукта включает множество видов **элементов**, в первую очередь новую пользовательскую функциональность (“разрешить всем пользователем класть книги в корзину”), цели по инженерному улучшению (например, “переписать код системы с C++ на Java”), улучшения (e.g. “ускорить наши тесты”), исследовательская работа (“исследовать решение для ускорения проверки кредитной карты”), и возможно, известные дефекты (“диагностировать и исправить ошибки порядка исполнения скриптов”), если только их немного (Системы с большим количество дефектов обычно имеют отдельную систему для их ведения).

Элементы Бэклога Продукта сформулированы в любом виде, понятном и устойчивом. Вразрез с популярным недопониманием Бэклог Продукта не содержит “пользовательские истории” (user stories); он просто состоит из *элементов*. Эти элементы могут быть выражены в формате пользовательских историй, сценариев использования или любом другом формате описания требований, который группа найдёт полезным. Но не важно, какой подход будет выбран, большинство элементы должны сконцентрироваться на поставке ценности клиентом.

Хороший Бэклог Продукта является ИСЧЕРПЫВАЮЩИМ...

**Подробно детализирован.** Самые приоритетные элементы наиболее хорошо прояснены и детализированы, чем остальные с более низким приоритетом, так как они попадут в работу раньше. Например, 10% верхушки Бэклога может состоять из очень небольших, хорошо проанализированных элементов, а остальные 90% из более крупных.

**Оценён.** The items for the current release need to have estimates, and furthermore, should be considered for re-estimation each Sprint as everyones learns and new information arises. The Team provides the Product Owner with *effort* estimates for each item on the Product Backlog, and perhaps also *technical risk* estimates. The Product Owner and other business stakeholders provide information on the value of the product  requests, which may include revenue gained, costs reduced, business risks, importance to various stakeholders, and more.

**Актуален.** In response to learning and variability, the Product Backlog is regularly refined. Each Sprint, items may be added, removed, modified, split, and changed in priority. Thus, the Product Backlog is continuously updated by the Product Owner to reflect changes in the needs of the customer, new ideas or insights, moves by the competition, technical hurdles that appear, and so forth.

**Приоритизирован.** The items at the top of the Product Backlog are prioritized or ordered in a 1-N order. In general, the highest-priority items should deliver the most *bang for your buck*: lots of bang (business value) for low buck (cost). Another motivation to increase the priority of an item is to *tackle high risks early, before the risks attack you.*

Traditional development does not usually emphasize delivering according to highest *bang for your buck*, but this is a theme of Scrum, and therefore the Product Owner will need to learn how to assess the bang of “business value.” This is something the Scrum Master may help the Product Owner learn. What does “business value” mean? Some product groups use a simple relative value-point estimate for each Product Backlog item which synthesizes a “guesstimate” of factors including revenue gain, cost reduction, stakeholder preferences, market differentiation, and so forth. Some fund a specific item by one or more customers paying for its development and so use that item's exact (short term) revenue as a proxy for value. For other groups such item-specific value estimation is too unfocused or granular; they apply a broader business-outcome-based approach ("increase subscriptions by 10% by September 1") in which value is only delivered when multiple outcome-contributing items are delivered together. In that case, the Product Owner needs to define the next increment of Minimum Viable Product.

For effort estimates, a common technique is to estimate in terms of relative size (factoring in effort, complexity, and uncertainty) using a unit of “story points” or simply “points”.

These are just suggestions; Scrum does not define the technique for expressing or prioritizing items in the Product Backlog and it does not define the estimation technique or units.

A common technique used in Scrum is to track how much work it completes each Sprint; for example, averaging 26 points completed per Sprint. With this information they can project a release date to complete all features, or how many features can be completed by a fixed date, if the average continues and nothing changes.  This average is called the “velocity.” Velocity is expressed in the same units as the Product Backlog item size estimates.

The items in the Product Backlog can vary significantly in size or effort. Larger ones are broken into smaller items during the Product Backlog Refinement workshop or the Sprint Planning Meeting, and smaller ones may be consolidated. The Product Backlog items for the upcoming next several Sprints should be small and fine-grained enough that they are understood by the Team, enabling forecasts made in the Sprint Planning meeting to be meaningful; this is called an “actionable” size.

Major engineering improvements that consume much time and money should be in the Product Backlog, since they may be an optional business investment, ultimately to be made by the business-oriented Product Owner. Note that in Scrum, the Team has independent authority of how many items from the Product Backlog they decide to take into a Sprint, so they are independently free to take on minor engineering improvement work as they can be considered part of the normal cost of doing business and what is required for a developer to do their job properly. That said, in each Sprint, the *majority* of a Team’s time should usually be on Product Owner goals, not internal engineering tasks.

One of the myths about Scrum is that it prevents you from writing detailed specifications; in reality, it is up to the Product Owner and Team to decide how much detail is required, and this will vary from one backlog item to the next, depending on the insight of the Team, and other factors. State what is important in the least amount of space necessary – in other words, do not describe every possible detail of an item, just make clear what is necessary for it to be understood, and augment this with continuous dialog between the Team and Product Owner and stakeholders. Low priority Product Backlog Items, which will not be worked on for some time, are usually “coarse grained” (large, with less-detailed requirements). High priority and fine-grained Product Backlog Items that will soon be implemented tend to have more detail.

Перевод статьи осуществлён [Кротовым Артёмом](https://www.facebook.com/artem.v.krotov) и [Романом Лапаевым](https://www.linkedin.com/in/romanlapaev).
