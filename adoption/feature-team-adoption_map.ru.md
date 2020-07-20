---
title: Карта Внедрения Фиче-Команд
order: 50
---

A feature team adoption map is a useful tool when adopting feature teams.

Карта внедрения фиче-команд является хорошим инструментом при внедрении фиче-команд. 

## Диаграмма масштаба и специализации

Что такое компонент? Что такое фича? Что такое функциональная специализация? До сих пор мы рассматривали их как двоичные, но ответ живёт вдоль континуума. Одна группа владеет одним классом в коде, тогда как другая группа владеет целой подсистемой. Они обе компонентные. Существует похожее измерение, относящееся к функциональной специализации, так некоторые продуктовые группы имеют пять уровней тестирования, для которых фраза “включите тестирование в команду” имеет очень неясное значение! Изображение этих измерений на графике даёт некоторое понимание во внедрении фиче-команд и виде организационных изменений, которые вы можете ожидать.

<div>
  {% figure "img/adoption/feature-team-adoption-map", "Feature Team Adoption Map" %}
</div>

График показывает четыре области:

* Компонентные команды — Любая команда, которая (1) фокусируется на части продукта, а не фичах, ориентированных на клиентах,  или (2) фокусируется на завершении задачи, а не поставке инкремента продукта является компонентной командой. Заметьте!…  Чем меньше масштаб владения и строже специализация, тем больше проблема компонентных команд.
* Фиче-команды — Любая команда, которая имеет фокус на всём продукте целиком и вовлечена в процесс от прояснения фич, ориентированных на клиента, до их тестирования является фиче-командой. Фиче-команды также существуют в измерении. Они могут быть ограничены в реализации предопределённых или вовлечены в выяснение и решении проблем реальных клиентов.
* Функциональная узкоспециалиазцированная команда — Любая команда, которая выполняет ограниченную задачу в рамках большого масштабе, вероятно, является узкоспециалиазцированной. Это ведёт к большому объему потерь, обусловленных передачами. Нужно это избегать.
* Расширенные компонентные команды — Любая команда that has a limited component ownership yet is responsible for checking that their part works within the larger product is an extended component team. The team has an internal conflict as they have both a limited “component scope” and a “whole product scope.” This conflict leads to either (1) duplication of work as multiple teams create the same tests, or (2) additional coordination effort as the teams have to coordinate their “product focused” testing. The same conflict of scope is true for requirements clarification. These teams are perhaps an improvement over basic component teams but fall far short of delivering the benefits of feature teams.

## Карта внедрения фиче-команд

A “perfect feature team” is a team that works across the whole system and co-creates the product together with actual users. This is a good very-difficult-to-achieve perfection goal.

With that perfection goal, we can use the earlier chart as a feature-team adoption map. Here is an example:

<div>
  {% figure "img/adoption/feature-team-adoption-map-telecom", "Feature Team Adoption Map - Example Telecom" %}
</div>

This feature-team adoption map is from a product adopting LeSS Huge. When they started their adoption they had traditional component teams. They chose the adoption strategy of expanding the teams functional scope and created extended component teams. Their goal for the next few years is to move to full product-wide feature teams. However there are some shared components created by a peer product group and that makes it hard to include these as it would require a significantly larger organizational change. So, these are excluded from their current goal.

Перевод статьи осуществлён [Кротовым Артёмом](https://www.facebook.com/artem.v.krotov).