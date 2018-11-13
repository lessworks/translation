---
layout: mechanics
title: Критерии Готовности
order: 87
---

Для эффективности циклов инспекции и адаптации Скраму нужна прозрачность. Формальное определение значения «Готово» уменьшает вариативность и сложность определения незаконченной работы, и однозначное определение прогресса («готово» или «не готово») повышает прозрачность.

Идеальные Критерии Готовности (Definition of Done) включает в себя всё что потребуется, чтобы организация доставила продукт клиентам. Достижение этого должны быть относительно простым для одной команды. Если команда неспособна достигать идеальных Критериев Готовности - она определяет свое Готово, как часть идеального Готово. Цель команды улучшаться так, чтобы в один из дней их Критерии Готовности стали идеальными, и они смогли доставлять продукт каждый Спринт или чаще.

Критерии Готовности - это согласованный список критериев которому соответствует программное обеспечение для каждого Элемента Бэклога Продукта. Достижение такого уровня полноты требует от Команды выполнения списка задач. Когда все задачи будут завершены, элемент будет готов. Не путайте критерии готовности с критериями приемки (acceptance criteria), которые являются частными условиями для приемки отдельного элемента. Критерии готовности применяется одинаково ко всем элементам Беклога Продукта.

## Создание Критериев Готовности

Первоначальное определение Критериев Готовности должно быть создано до первого Спринта. Обычно это происходит на [Первом Уточнении Бэклога Продукта](initial-product-backlog-refinement.html).

Следующие шаги предпринимаются для создания Критериев Готовности:
* Определить необходимые действия чтобы доставить до конечных пользователей.
* Решить какие действия могут быть выполнены каждый Спринт.

Давайте рассмотрим эти шаги более подробно.

### Определить необходимые действия чтобы доставить до конечных пользователей

Главный вопрос “Какие действия необходимо сейчас выполнить чтобы доставить наш продукт?”

* Доставить означает “доставить до конечных пользователей”, а никак не “отправить в департамент разработки.”
* Обсудить необходимость в промежуточных артефактах. Действительно ли нам нужны эти документы спецификаций?

Команды записывают на стикерах необходимые действия. К ним относятся такие виды деятельности, как кодирование и тестирование, но также могут включать настройку поддержки клиентов, создание оборудования или даже маркетинговую деятельность. Мы ссылаемся на данный список как на необходимые действия для получения потенциально готового к поставке продукта (Potentially Shippable Product).

На этом этапе вы создали [цель совершенства](../principles/continuous-improvement-towards-perfection.html) для организации - выполнение всех действий для каждого элемента в каждом Спринте. Продуктовые группы часто понимают, что это принесет много улучшений.

### Решить какие действия могут быть выполнены каждый Спринт.

Главный вопрос: “Учитывая наш текущий контекст и возможности, какие действия могут быть выполнены каждый Спринт?” Это будет являться частью первоначальных Критериев Готовности Критерии Готовности слабы если они являются лишь малой частью и сильны когда почти равны определению "готовому к поставке".

Команды обсуждают свой контекст и выбирают ту часть действий, которые они могут реально делать во время Спринта, по мнению всех команд. Это их первоначальные Критерии Готовности (см. пример на рисунке 1). Команды, которые могут сделать больше будут расширять их частные Критерии Готовности.

Разница между Критериями Готовности и Готовым к Поставке называется Неготовой Работой. Планирование Спринта проходит с учетом Критериев Готовности и исключением Неготовой Работы - её планируется оставить неготовой.

<div>
  {% figure_with_caption "/img/framework/dod", "Рисунок 1. Потенциально готовый к поставке и Критерии Готовности.  %}
</div>

## Терминология Критериев Готовности

Термины Потенциально Готовый к Поставке и Критерии Готовности часто не используются последовательно, но в LeSS они имеют очень точное значение. Уточним термины:

**Потенциально Готовый к поставке** - Все действия, которые должны быть выполнены для поставки продукта.

**Критерии Готовности** - Соглашение между командами и Владельцем Продукта о том, какие из действий выполняются внутри Спринта. Критерии Готовности идеальны, когда они равны определению Потенциального Готового к Поставке. Команды стремятся улучшаться в сторону идеальных Критериев Готовности.

**Неготовая Работа** - Разница между определениями Критериями Готово и Потенциально готовым к поставке. Неготовой Работы нет, когда Критерии Готовности идеальны. Если же это не так, то организация должна решить, (1) что мы делаем с Неготовой Работой, и (2) Как нам улучшаться, чтобы в будущем было меньше Неготовой Работы.

**Незавершенный, несделанный или незаконченный** - Работа, которая была запланирована в Спринт, но не была завершена. Это часто путают с Неготовой Работой. 'Незавершенная' - это работа, которую команда планировала, но не закончила, в то время как Неготовая Работа никогда и не планировалась. Когда у команды есть работа, которую она хотела завершить, но не завершила, оно должна быть обеспокоена и обсудить действия по улучшению во время Ретроспективы.

Команды не должны оставлять работу-в-процессе под конец Спринта и "переносить" её на следующий. Это приводит к отсутствию прозрачности и уменьшению гибкости. Если они прогнозируют слишком много работы, им необходимо удалить цельные элементы, которые еще не были начали.

### Математика определения Готово

Потенциально Готовый к Поставке = Критерии Готовности + Неготовая Работа
Работа в Итерации = Элемент Бэклога Продукта * Критерии Готовности
{: .box_top_bottom  .text_centered_bold }

## Неготовая Работа -> Риски и Задержки

Давайте сначала рассмотрим эффекты Неготовой Работы на примере сценария.

Команды завершили - в соответствии с Критериями Готовности - двадцать Элементов Бэклога Продукта в первом Спринте. У них нет незавершенной работы, но есть много Неготовой Работы из-за слабых Критериев Готовности. Позднее команды завершили - в соответствии со слабыми Критериями Готовности - сорок Элементов Бэклога Продукта в трех Спринта. Количество Неготовой Работы существенно увеличилось, создавая ложное чувство прогресса.

Но они не могут поставить продукт. Они "сделали" фичи, но их слабые Критерии Готовности привели к накоплению огромного количества Неготовой Работы. Эта Неготовая Работа вызвала задержку и скрытый риск.

**Задержка** - Дополнительные усилия необходимые для работы с Неготовой Работой. Это приводит к отсутствию гибкости, нужной Владельцу Продукта - он не может напрямую реагировать на изменения и потребности рынка. Боль, вызванная этой задержкой, усугубляется тем фактом, что усилия по завершению Неготовой Работы сильно варьируются и их трудно предсказать.

**Риск** - Неготовая Работа вызывает отсутствие прозрачности. В этом скрываются риски. Например, если тестирование производительности оставлено Неготовым, это задерживает риск неработоспособной системы до тех пор, пока она не будет выпущена - когда это сильно больно.

Хороший Владелец продукта хочет идеальное Определения Готово так как это снижает продуктовые риски и устраняет задержки.

Перевод статьи осуществлен [Иваном Переслегиным](https://www.facebook.com/pereslegin)