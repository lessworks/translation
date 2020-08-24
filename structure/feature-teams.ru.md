---
title: Фиче-команды
order: 30
---

Фиче-команда, изображённая на первой иллюстрации, является долгоживущей, кросс-функциональной командой, которая выполняет множество задач, описанных пользовательским языком - одна за одной. 

<div>
  {% figure "img/structure/feature-team", "Фиче-команда" %}
</div>

Свойства фиче-команды показаны ниже:

* долгоживущая - команда остаётся вместе, поэтому они могут ‘застыть’ для достижения высокой производительности; со временем они приобретают новые свойства
* кросс-функциональная и кросс-компонентная
* колоцированная
* работает над задачей, описанной клиентским языков, до её завершения, во всех компонентах и дисциплинах (аналитика, программирование, тестирование, …)
* состоит из специалистов широкого профиля
* как и в Скраме обычно состоит из 7 ± 2 человек

Применение современных инженерных практик - особенно непрерывной интеграции - является самым важным при переходе к фиче-командам. Непрерывная интеграция помогает общему владению кодом, которое необходимо, когда несколько команд работают над одними и теми же компонентами в одно и то же время. 

Типичное заблуждение: каждый член фиче-команды должен знать всю систему целиком. Но это не так, потому что

* Команда целиком - а не каждый член в отдельности - требует всех навыков для выполнения задач, ориентированных на клиента. Они включают в себя знания и функциональные навыки, такие как тестирование, проектирование взаимодействия или программирование. Но внутри команды люди по-прежнему специализируются… желательно в нескольких областях.
* Задачи Бэклога Продукта не распределяются между командами произвольно. Текущие знания и навыки команды учитываются в принятии решения, какая команда будет работать над какими задачами. 

В организации, состоящей из фиче-команд, когда специализация становится ограничением… тогда происходит обучение.

*Организация, состоящая из фиче-команд, использует преимущества в скорости от специализации, если требования покрываются навыкам команд.
Но когда требования не соответствуют навыкам команд, тогда обучение ’ускоряется’, разрушая ограничения чрезмерной специализации.
Фиче-команды сочетают в себе специализацию и гибкость.*
{: .box_top_bottom  .text_centered_bold }

# сравнение компонентных и фиче-команд

Таблица ниже и вторая иллюстрация показывают отличия фиче-команд и более традиционных компонентных команд.

| компонентная команда                                                                           | фиче-команда                                        |
|:----------------------------------------------------------------------------------------------:|:---------------------------------------------------:|
| оптимизирована для поставку максимального числа строк кода                                     | оптимизирована на поставку максимальной клиентской ценности |
| фокус на увеличении индивидуальной продуктивности, разрабатывая ‘лёгкие’ низкоуровневые задачи | фокус на самых ценных для продукта задачах и продуктивности системы (пропускной способности доставки ценности) |
| несёт ответственность только за часть задачи, ориентированной на клиента                       | несёт ответственность за всю задачу, ориентированную на клиента,  целиком
| традиционный подход организации команд — следует Закона Конвея                                 | ‘современный’ подход организации команда — избегает Закона Конвея  |
| ведёт к ‘изобретению’ работы и бесконечно растущей организации                                 | ведёт к фокусу не клиенте, прозрачности, и небольшим организациям |
| зависимости между командами ведут к дополнительному планированию                               | минимизируют зависимости между командами, увеличивая гибкость |
| фокус на одной специализации                                                                   | фокус на нескольких специализациях |
| индивидуальное/командное владение кодом                                                        | общее владение кодом продукта |
| чёткая индивидуальные ответственность                                                          | общая командная ответственность |
| выражается в ‘каскадной’ разработке                                                            | поддерживает итеративную разработку |
| использует существующую экспертизу; низкий уровень изучения новых навыков                      | использует гибкость; непрерывное и широкое обучение |
| работает с инженерными практиками небрежно — эффект от них локализован                         | требует развитых инженерных практик — эффект от них широко заметен   |
| вопреки убеждению часто ведёт к низкому качеству кода в компоненте                             | мотивирует писать легко поддерживаемый и тестируемый код|
| создать, по-видимому, легко                                                                    | создать, по-видимому, тяжело |
{: .grid_table_with_header}

<div>
  {% figure "img/structure/component-vs-feature-teams", "Сравнение Компонентных и Фиче-команд" %}
</div>

Таблица ниже подводит итоги в сравнении фиче-команд и обычных проектных или специализированных групп.

| feature team                                                          | feature group or feature project |
|:---------------------------------------------------------------------:|:--------------------------------:|
| stable team that stays together for years and works on many features  | temporary group of people created for one feature or project |
| shared team responsibility for all the work	                          | individual responsibility for ‘their’ part based on specialization |
| self-managing team                                                    | controlled by a project manager |
| results in a simple single-line organization (no matrix!)             | results in a matrix organization with resource pools |
| team members are dedicated—100% allocated—to the team                 | members are part-time on many projects because of specialization |
{: .grid_table_with_header}

Most drawbacks of component teams are explored in the “Feature Teams” chapter of Scaling Lean & Agile Development, Figure 3 summarizes some of these.

<figure>
  <img src="/img/feature-teams/component_teams_waterfall.png" alt="component_teams_waterfall.png">
  <figcaption>Figure 3. Some Drawbacks of Component Teams.</figcaption>
</figure>

What is sometimes not seen is that a component team structure reinforces sequential development (a ‘waterfall’ or V-model), with many queues with varying-sized work packages, high levels of WIP, many handoffs, and increased multitasking and partial allocation.

## Что выбрать: Компонентные Команды или Фиче-команды?

A pure feature team organization is ideal from the value-delivery and organizational-flexibility perspective. Value and flexibility, however, are not the only criterion for organizational design, and many organizations therefore end up with a hybrid—especially during a transition from component to feature teams. Caution: hybrid models have the drawbacks from both worlds and can be…painful.

A frequently expressed reason in favor of a hybrid organization is the need to build infrastructure, construct reusable components, or clean up code—work traditionally done within component teams. But these activities can also be done in a pure feature team organization—without establishing permanent component teams. How? By adding infrastructure, reusable components, or cleanup work to the Product Backlog and giving it to an existing feature team—as if it were a customer-centric feature. The feature team temporarily—for as long as the Product Owner wishes—does such work and then returns to building customer-centric features.

## Переход к Фиче-командам

Different organizations require different transition strategies when changing from component to feature teams. We have experience with many strategies that worked…and failed in a different context. A safe—but slow—transitioning strategy is to establish one feature team within the existing component team organization. After this team performs well, a second feature team is formed. This continues gradually at the speed the organization is comfortable with. This is shown in Figure 4.

<div>
  {% figure "img/feature-teams/transition-component-teams-slow", "Gradual Slow Transition to Feature Teams" %}
</div>

## Рекомендуем к Прочтению

* Feature Team Primer
  This article originally appeared as the [Feature Team Primer](http://www.featureteamprimer.com/)
* Feature Teams chapter of [Scaling Agile & Lean Development](http://www.amazon.com/Scaling-Lean-Agile-Development-Organizational/dp/0321480961)
  This 60-page analysis of feature and component teams is also [available online](https://res.infoq.com/articles/scaling-lean-agile-feature-teams/en/resources/feature%20teams_%20infoq_%20final.pdf)
* [Dynamics of Software Development by Jim McCarthy](http://www.amazon.com/Dynamics-Software-Development-Jim-McCarthy/dp/1556158238)
  Originally published in 1995 but republished in 2008. Jim’s book is a true classic on software development. Already in 1995 it emphasized feature teams. The rest of the book is stuffed with insightful tips related to software development.
* [“XP and Large Distributed Software Projects” by Karlsson and Andersson.](_http://dl.acm.org/citation.cfm?id=377525_)
  This early large-scale agile development article is published in Extreme Programming Perspectives. It is a insightful and much under-appreciated article describing the strong relationship between feature teams and continuous integration.
* [“How Do Committees Invent?” by Mel Conway.](http://www.melconway.com/research/committees.html)
  This 40-year article is as insightful today as it was 40 years ago. It is available via the authors website at www.melconway.com.