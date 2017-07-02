---
layout: mechanics
title: Знакомство с LeSS
order: 5
---
(это глава 2 из [книги "Large-Scale Scrum: More with LeSS" ISBN 9780321985712](http://www.amazon.com/Large-Scale-Scrum-More-Craig-Larman/dp/0321985710))

<div class="chapter_quote"><p>
There are two ways of constructing a [design]:
Есть два пути проектирования [конструирования]:
<br/>
Один путь - сделать все настолько просто, что очевидно не будет недостатков.
<br/>
И другой - сделать все настолько сложно, что не будет очевидных недостатков.
<br/>
C.A.R. Hoare
</p></div>

## Скрам для одной команды

 Скрам - это процессный фреймворк, основанный на теории эмпирического управления, в рамках которого самоуправляемая кросс-функциональная команда разрабатывает продукт, следуя итеративно-инкрементальному подходу. По итогам каждого, ограниченного во времени, *Спринта* разрабатывается (а в идеале - поставляется) *инкремент продукта, потенциально готовый к поставке*. Единственный *Владелец Продукта* отвечает за максимизацию ценности продукта, с помощью приоритизации *элементов* *Бэклога Продукта* и постановку цели для каждого Спринта, основываясь на постоянной обратной связи от заинтересованных лиц и конечных пользователей. За достижение цели Спринта отвечает небольшая *Команда*, в которой нет жестко огрганичивающих одной специализацией ролей. *Скрам-мастер* обучает Владельца Продукта, Команду и в целом организацию Скраму и как с его помощью поставлять ценность, и выполняет роль “зеркала” для команды. В Скраме нет менеджера проекта или лидера команды.

Эмпирический контроль процесса требует *прозрачности*, которая достигается путем разработки и ревью готового к поставке инкремента продукта короткими циклами. В нем делается акцент на непрерывное обучение, инспекцию и адаптацию подхода к созданию продукта. В его основе лежит понимание того, что в разработке все настолько комплексно (запутанно) и быстро меняется, что использование детализированного и шаблонного процесса препятствует вовлечению и постоянным улучшениям.

В [Руководстве по Скраму (Scrum Guide)](http://www.scrumguides.org/) и [Азбуке Скрам (Scrum Primer)](http://scrumprimer.org/) делается акцент на работу одной команды, а не на совместную работу нескольких команд. Это естественным образом ведет к размышлениям о реализации Скрама в *больших масштабах*.

## LeSS

LeSS - это Скрам, применяемый к множеству команд, работающих совместно над одним продуктом
{: .box_top_bottom .text_centered_bold }

**LeSS - это Скрам**. Скрам на больших масштабах (LeSS / Large-Scale Scrum) - это не новый или улучшенный Скрам. И это не разделение на *Скрам на уровне каждой команды* и *что-то другое на уровне выше*. Скорее это о том, как применить принципы, назначение, элементы и элегантность Скрама в контексте большого масштаба настолько просто, насколько это возможно. Так же, как Скрам или любой другой настоящий Agile-фреймворк, LeSS является “минимально достаточным подходом” для максимальной отдачи.

> Скрам на больших масштабах - это не специальный фреймворк расширения, работающий только на уровне команд. По-настоящему масштабированный Скрам - это тот же Скрам, но работающий на большем масштабе.

**…применяемый к большому числу команд:** - Имея в виду кросс-функциональные, кросс-компонентные, обладающие всеми необходимыми компетенциями продуктовые команды (feature-team), состоящие из 3-9 нацеленных на обучение участников, выполняющих всю работу (от пользовательских интерфейсов и программирования до записи видео) для создания полноценного рабочего продукта.

**…работающих вместе:** - Команды работают вместе, потому что у них есть общая цель: по итогам общего Спринта разработать единый, цельный, готовый к поставке продукт, и каждая команда вовлечена в это, потому что она является продуктовой командой (feature-team), и отвечает за **цельный продукт**, а не только за его отдельную часть.

**…над одним продуктом:** - Каким продуктом? Полноценным (end-to-end), клиент-ориентированным решением, которое будет использоваться реальными людьми. Понятие продукта гораздо шире, чем просто компонент, платформа, слой или библиотека.

### • Предистория •

В 2002 году, когда Крэг Ларман написал книгу [Agile & Iterative Development](https://www.amazon.com/Agile-Iterative-Development-Managers-Guide/dp/0131111558), многие считали, что Agile применим только для небольших групп. Однако, мы оба (Крэг Ларман и Бас Водд) начали интересоваться - и стали получать большое количество запросов - в применении Скрама на больших масштабах, в мультилокационной среде и и в офшорной разработке. Так, начиная с 2005 года, мы объединились для совместной работы по масштабированию Скрама у крупных клиентов. На сегодняшний день два LeSS фреймворка ([smaller LeSS](https://less.works/less/framework/index.html) и [LeSS Huge](https://less.works/less/less-huge/index.html)) применяются в больших компаниях по всему миру в различных отраслях:

* телекоммуникационное оборудование - Ericsson и Nokia Networks;
* инвестиции и розничные банки - UBS;
* трейдерские площадки - ION Trading;
* маркетинговые платформы и бренд-аналитика - Vendasta;
* видеоконференции - Cisco;
* онлайн-игры (ставки) - bwin.party;
* зарубежный аутсорсинг - Valtech India.

Насколько масштабным является типовой [кейс внедрения](https://less.works/case-studies/index.html) LeSS? В среднем, около пяти команд на одной или двух площадках. Мы участвовали во внедрениях LeSS на подобных объемах, на объемах в несколько сотен человек, и до более чем тысячи человек в случае LeSS Huge, с очень большим числом распределенных команд разработки, десяткам миллионов строк кода на C++ и заказным, адаптированным под клиента, системным оборудованием.

#### Больше о LeSS

Для помощи людям в изучении LeSS, в 2008 и 2010 годах мы опубликовали две книги о масштабировании Agile разработки с помощью фреймворка LeSS, которые основаны на нашем опыте работы с клиентами:

1. [Scaling Lean & Agile Development: Thinking and Organizational Tools for Large-Scale Scrum](https://www.amazon.com/Scaling-Lean-Agile-Development-Organizational/dp/0321480961) - описывает изменения в мышлении, лидерстве и подходах к организационному дизайну.
2. [Practices for Scaling Lean & Agile Development: Large, Multisite & Offshore Product Development with Large-Scale Scrum](https://www.amazon.com/Practices-Scaling-Lean-Agile-Development/dp/0321636406) - в этой книге мы делимся результатами нескольких сотен реальных экспериментов с LeSS, полученных при работе с нашими клиентами, включая управление продуктом, дизайн архитектуры решения, планирование, распределенную работу, специфику контрактов и т.д.

Книга - [Large-Scale Scrum: More with LeSS](https://www.amazon.com/Large-Scale-Scrum-More-Addison-Wesley-Signature/dp/0321985710) - третья в серии, описывает предысторию и основы фреймворка LeSS. Она формулирует, разъясняет и подчеркивает его наиболее важные аспекты.

Помимо этих книг, рекомендуем сайт [less.works](https://less.works), как ресурс для онлайн-обучения (включает главы книг, статьи и видео), курсов и коучинга.

### • Эксперименты, Руководства, Правила, Принципы •

Первые [две книги по LeSS](https://less.works/resources/books.html) подчеркивали: *в продуктовой разработке нет такого понятия как “лучшие практики” - есть только практики, применение которых целесообразно в конкретном контексте*.

Практики ситуационны, и беспечное объявление их “лучшими” отрывает их от мотивации и контекста. Они превращаются в ритуалы, и навязывание так называемых “best practices” убивает культуру обучения, задавания вопросов, вовлечения и непрерывных улучшений. Зачем людям искать чего-то лучшего, если все уже придумано за них?

В наших ранних книгах по LeSS мы делились результатами *экспериментов*, которые мы пробовали совместно с нашими клиентами, и мы вдохновлялись этим подходом. Но, по прошествии времени, мы обнаружили две проблемы, связанные с применением подхода, основанного исключительно на экспериментах:

* Неопытные команды принимали некомпетентные решения, применяя LeSS не по назначению, с очевидными ошибками. Например, они создавали Области Требований (Requirement Areas), каждая из которых состояла из одной команды. Ой!
* Неопытные команды спрашивали: “С чего нам следует начинать? Что является наиболее важным?” Они, очевидно, не могли увидеть и понять базовые принципы.

Получив такую обратную связь, мы поразмыслили и вернулись к японской модели изучения [Сю-Ха-Ри](https://ru.wikipedia.org/wiki/сюхари): *Сю* - следуй правилам, чтобы изучить основы, *Ха* - нарушай правила и изучай обстановку, *Ри* - создавай и ищи собственный путь. На Сю-уровне понимания LeSS есть *несколько правил для внедрения минимально достаточного* фреймворка, чтобы запустить эмпирический контроль  процесса и создать фокус на всем продукте. Эти правила определяют два **LeSS-фреймворка**, которые будут представлены ниже.

Суммируя сказанное, LeSS включает в себя:

* **Правила** – [несколько правил](https://less.works/less/rules/index.html), чтобы начать работу и сформировать основу. Они определяют ключевые элементы **фреймворков LeSS**, которые должны быть реализованы для поддержки эмпирического контроля над процессом и фокуса на всем продукте. Например, *Проводите Общую Ретроспективу (Overall Retrospective) каждого Спринта*.
* **Руководства** – набор рекомендаций для эффективного применения правил и для ограниченного числа конкретных экспериментов, которые доказали свою эффективность в нашем многолетнем опыте с LeSS. Рекомендации содержат *полезные советы*, которые могут помочь понять область для дальнейших улучшений. Например, *Три принципа внедрения*.
* **Эксперименты** – множество наших экспериментов, которые были очень ситуационными и которые, возможно, даже не следует повторять. Например,*Попробуйте… переводчика для мультиязычной команды*.
* **Принципы** – и, в центре всего, [набор принципов](https://less.works/less/principles/index.html), выработанных на основании нашего опыта внедрения LeSS, и являющихся основой для Правил, Рекомендаций и Экспериментов. Например, *фокус на всем продукте*.

Руководства LeSS и Эксперименты не являются обязательными к выполнению. Руководства могут быть полезными, и мы рекомендуем их попробовать. Но смело пропускайте те из них, которые ограничивают вас в дальнейших улучшениях или просто вам не подходят.
{: .box_top_bottom .text_centered_bold }

Хороший способ представить LeSS приведен ниже на рисунке *Верхнеуровневый взгляд на LeSS*:

<div>
  {% figure "img/framework/less-complete-picture", "The LeSS Complete Picture", class:"half-sized-figure" %}
</div>

Дальнейший рассказ о LeSS мы построим в соответствии с этим рисунком:

1. LeSS **Принципы**, непосредственно следующий раздел.
2. LeSS **Фреймворки** (определяются [правилами](https://less.works/less/rules/index.html)) - в оставшейся части данной главы.
3. LeSS **Руководства** - в оставшихся главах книги.
4. LeSS **Эксперименты** - описаны в первых двух книгах.

### • Принципы LeSS •

[Правила LeSS](https://less.works/less/rules/index.html) определяют LeSS-фреймворк. Но правила очень минималистичны и не отвечают на вопрос, как следует применить LeSS в вашем конкретном случае. [Принципы LeSS](https://less.works/less/principles/index.html), в отличие от правил, предоставляют основу для принятия таких решений.

<div>
  {% figure "img/principles/principles", "LeSS Principles" %}
</div>

[**Масштабированный Скрам – это Скрам (Large-Scale Scrum is Scrum)**](https://less.works/less/principles/large_scale_scrum_is_scrum.html) - Это не новый или улучшенный Скрам. Напротив, LeSS позволяет понять, как применить Принципы, Правила, Элементы и базовую цель Скрам в масштабе настолько просто, насколько это возможно.

[**Прозрачность (Transparency)**](https://less.works/less/principles/transparency.html) - Прозрачность базируется на осязаемых результатах, коротких циклах разработки, командной работе, общей терминологии и устранении страха на рабочих местах.

[**Больше за счет меньшего (More with less)**](https://less.works/less/principles/more-with-less.html) - Нам не нужно **больше ролей**, потому что наличие большого числа ролей приводит к меньшей ответственности Команд. Нам не нужно **больше артефактов**, потому что большое число артефактов приводит к увеличению дистанции между Командами и Клиентом. Нам не нужно **больше процессов**, потому что формализация губит желание обучаться, и Команды перестают отвечать за процесс. Взамен мы хотим **более ответственные Команды**, за счёт введения меньшего числа ролей; мы хотим **более сфокусированные на нуждах клиента команды**, которые создают полезные продукты, порождая небольшое число артефактов; мы хотим **больше командной ответственности и больше значимой работы** за счет исключения лишнего формализма в процессах. *Мы хотим больше за счет меньшего (“more with less”)*.

[**Фокус на всем продукте (Whole-product focus)**](https://less.works/less/principles/whole-product-focus.html) - Один Бэклог Продукта, один Владелец Продукта, один Поставляемый Продукт, один общий Спринт – вне зависимости от того, работают ли совместно 3 или 33 команды. Клиенты получают ценность от всего продукта, а не в отдельности от его  технических компонентов.

[**Ориентация на клиента (Customer-centric)**](https://less.works/less/principles/customer-centric.html) - Фокус на изучение реальных проблем клиента и их решение. Определение того, что ценно, а что нет, в глазах клиента. Снижение времени ожидания с точки зрения клиента. Усиление петель обратной связи от реальных потребителей. Необходимо, чтобы каждый член команды понимал, как их совместная работа сегодня приносит пользу клиентам, приобретающим продукт.

[**Непрерывные улучшения на пути к совершенству (Continuous improvement towards perfection)**](https://less.works/less/principles/continuous-improvement-towards-perfection.html) - Вот наша цель на пути к совершенству: создавать и поставлять продукт практически непрерывно, с минимальными затратами, без дефектов; продукт, который восхищает клиентов и делает их жизнь лучше. Практикуйте непрерывные, небольшие и радикальные эксперименты по улучшению на пути к этой цели.

[**Lean-мышление (Lean Thinking)**](https://less.works/less/principles/lean-thinking.html) - Создайте такую организационную систему, основой которой будут руководители-учителя, применяющие и прививающие Lean-мышление, практикующие управление, направленное на улучшения, поощряющие подход “остановись и исправь”, которые используют подход “Иди и посмотри” (Go See - подход Тойота, когда менеджер присутствует там где непосредственно происходит выполнение работы). Два столпа такого управления – это уважение к людям и мышление, направленное на постоянный поиск улучшений текущего положения вещей. Все на пути к совершенству.

[**Системное мышление (System Thinking)**](https://less.works/less/principles/systems-thinking.html) - Наблюдайте, старайтесь понять и оптимизировать систему в целом, а не по частям, и используйте средства системного моделирования для изучения ее динамики. Избегайте локальных оптимизаций, нацеленных на повышение эффективности или продуктивности конкретного члена команды или конкретной команды. Клиенты заботятся об оптимизации времени от идеи до реальной прибыли для продукта целиком, а не для его отдельных частей, а локальная оптимизация *отдельной части* в отрыве от целого практически всегда приводит к снижению производительности *всей системы*.

[**Эмпирический контроль процесса (Empirical process control)**](https://less.works/less/principles/empirical-process-control.html) - Непрерывно инспектируйте и адаптируйте продукт, процессы, поведение, организационную структуру и практики, чтобы развиваться в направлении, адекватном текущей ситуации. Делайте это вместо того, чтобы следовать прописанным, так называемым “лучшим” практикам, игнорируя контекст, вместо слепого следования ритуалам, которое препятствует обучению и изменениям и снижает тем самым вовлеченность и ответственность людей в компании.

[**Применение теории массового обслуживания (Queuing theory)**](https://less.works/less/principles/queueing_theory.html) - Изучайте, как методы работы с очередями могут быть применены в R&D домене, и применяйте полученные знания в управлении размером очередей, ограничениями на количество незавершенной работы, многозадачностью, размерами работ и вариативностью.

### • Два каркаса: LeSS и LeSS Huge •

Скрам на больших масштабах состоит из двух фреймворков:

* [**LeSS**](https://less.works/less/framework/index.html) - от 2 до 8 команд
* [**LeSS Huge**](https://less.works/less/less-huge/index.html) - 8+ команд

При этом сам термин *LeSS* несколько перегружен и означает как Скрам на больших масштабах в целом, так и обычный LeSS-фреймворк до 8 команд.

#### Магическое число восемь

В действительности *число восемь* не является магическим, и, если ваша компания может успешно применять обычный LeSS-фреймворк на числе команд, большем восьми, прекрасно! Но мы с таким не встречались… пока. Это только наше практическое наблюдение. В некоторых случаях, при наличии нескольких сложных целей и распределенных-мультиязычных-неопытных команд, эта граница может быть даже меньше восьми.

В любом случае, в какой-то момент, когда (1) один Владелец Продукта более не может держать в голове полный контекст, (2) у Владельца Продукта более не получается соблюдать баланс между внутренними и внешними коммуникациями и (3) Бэклог Продукта разрастается настолько, что один человек более не способен с ним справляться.

Когда компания достигает этой критической точки, возможно, это сигнал для перехода от обычного LeSS к LeSS Huge. Однако, перед этим мы рекомендуем пробовать внутренние изменения, чтобы стать лучше, меньше и проще, прежде чем двигаться в сторону *укрупнения*.

#### Общее для двух каркасов LeSS

LeSS и LeSS Huge имеют следующие общие элементы:

* Один Владелец Продукта и один Бэклог Продукта;
* Один общий Спринт для всех команд;
* Один поставляемый инкремент продукта.

Следующие два раздела данной главы детально описывают эти фреймворки, сначала меньший LeSS, затем LeSS Huge [далее в](#less-huge-framework).

## Каркас LeSS

### • Коротко о каркасе LeSS •

<div>
  {% figure "img/framework/less-framework", "LeSS Framework" %}
</div>

Меньший LeSS-каркас подразумевает одного (и только одного) Владельца Продукта, который владеет продуктом, оптимизируя продукт в целом, и управляет одним Бэклогом Продукта, над которым работают команды в рамках общего для всех Спринта. Элементы LeSS-фреймворка практически идентичны элементам Скрам для одной команды:

**Роли** - Один *Владелец Продукта*, от двух до восьми *Команд*, *Скрам Мастер*, сопровождающий от одной до трех команд. Важно, чтобы эти команды были продуктовыми командами (feature team) – действительно кросс-функциональными и кросс-компонентными командами, которые работают совместно в едином пространстве кода и каждая из них делает *всё*, чтобы создать полностью *готовый элемент бэклога продукта*.

**Артефакты** - Один *инкремент продукта, потенциально готовый к поставке*; один *Бэклог Продукта* и отдельный *Бэклог Спринта* для каждой *Команды*.

**События** - Один общий *Спринт* для всего продукта, он охватывает все команды и в качестве результата дает один *потенциально готовый к поставке инкремент продукта*. События будут детально рассмотрены в историях ниже и в отдельных главах.

**Правила и Руководства** - Правила описывают минимально достаточный фреймворк для обеспечения *эмпирического контроля над процессом* и *фокуса на всем продукте*. Руководства могут помочь вам в внедрении LeSS.

### • LeSS Истории •

**Изучение LeSS**—один из вариантов изучения - это чтение глубокого описания теоретической части, если вам предпочтительнее такой путь, то выможете пропустить эту часть и перейти к разделу [LeSS Huge](#less-huge-framework) и далее к последующим главам. Но, если вы любите истории и примеры из жизни, то это глава для вас.

**Простые истории**— истории, описанные ниже, не покрывают сложные аспекты разработки на больших масштабах, от политики до приоритизации, с которыми мы сталкиваемся в нашей консалтинговой работе, - они раскрываются в следующий главах. Сюда же мы намеренно включили простые истории, только чтобы показать базовые принципы Спринта LeSS. Если вы ищете захватывающих диалогов или драмы, то почитайте лучше книгу *Lean*.

**Правила и Руководства**— внутри каждой истории вы увидите отсылки на правила и руководства, которые используются в рамках данной ситуации. Это сделано, чтобы вы смогли отследить четкую связь между правилами, руководствами и рассматриваемым примером ситуации.

**Два ракурса**—для того, чтобы вам было проще ознакомиться с динамикой работы в LeSS, ниже вы найдёте две связанные истории, рассматривающие ситуацию с двух основных ракусов: 

1. [Динамика работы и взаимодействия команд в ходе LeSS Спринта.](#less-story-flow-of-teams-)
2. [Динамика клиентоориентированных элементов бэклога (features) в ходе LeSS Спринта.](#less-story-flow-of-items-)

### • LeSS История: Поток работы команд •

> Эта история больше фокусируется на работе *команд* в течение Спринта, чем на динамике элементов бэклога. На практике большую часть Спринта команды тратят на задачи разработки, а не на *встречи и совещания*, однако эта история намеренно делает акцент на взаимодействии, так как её целью является показать, как несколько команд вместе работают в ходе событий LeSS и как происходит их ежедневная координация.

Марк заходит в комнату, где работает его команда (Продажи), и видит Миру, которая встречает его словами: “Доброе утро! Хочу напомнить, что в этом Спринте мы с тобой являемся представителями нашей команды, и сессия Первого Планирования Спринта начнется через 10 минут”. “Хорошо”, - отвечает Марк, - “Встретимся в большой переговорной”.

#### Планирование Спринта Часть 1

Настало время для Первой Части Планирования Спринта, и в комнате собрались десять представителей пяти команд продуктовой группы. Все вместе они работают над флагманским продуктом компании по продаже облигаций и деривативов. Сэм, Скрам-мастер команд Trade и Margin, тоже присутствует на встрече. Он планирует наблюдать за обсуждением и подключаться как коуч, если потребуется. (ПРАВИЛО: Существует единственный общий продуктовый спринт для всех команд, а не отдельные спринты для каждой из команд).

Много Спринтов назад на Первой Части Планирования Спринта присутствовали все участники команд. Такой формат был более полезным пока участники команд еще не научились эффективно прояснять задачи и подготавливать их к работе, а также не наладили обмен знаниями о продукте между командами.
На этой встрече звучали ответы на множество вопросов, которые должен был услышать каждый. Со временем ситуация улучшилась, и сейчас группа экспериментирует, приглашая на эти встречи меняющихся из раза в раз представителей команд, благодаря чему встреча стала проходить просто и быстро. Обычно на ней поднимается и обсуждается всего несколько вопросов. Если такой новый подход не заработает, этот вопрос, вероятно, будет поднят на Общей Ретроспективе, и будет инициирован другой эксперимент по Планированию Спринта. (ПРАВИЛО: Планирование спринта состоит из двух частей. Первая Часть Планирования Спринта является общей для всех команд, в то время как Вторая Часть Планирования Спринта обычно осуществляется каждой из команд по отдельности. В случае связанных элементов бэклога проводите Межкомандную Вторую Часть Планирования Спринта.).

<div>
  {% figure "img/framework/sprint-planning-one-sketch", "Sprint Planning One - Story Sketch", class:"half-sized-figure pull-right" %}
</div>

Вот в комнату заходит Паоло и приветствует собравшихся. Паоло является Владельцем Продукта, а также ведущим продукт-менеджером. Он раскладывает на столе 22 карточки и комментирует: “Вот наши главные темы: немецкий рынок, управление заказами и несколько регуляторных отчётов. Я разложил их в соответствии с их приоритетами. Полагаю, каждый из вас понимает, почему приоритеты именно такие, поскольку мы уже довольно долго обсуждали это в ходе сессий по Уточнению Бэклога Продукта. Но, пожалуйста, не стесняйтесь переспросить, если вам что-то не понятно”. (ПРАВИЛО: На Первой Части Планирования Спринта присутствуют Владелец Продукта и Команды, либо представители команд. Они ориентировочно выбирают те элементы бэклога, над которыми будет работать каждая из команд. Команды проясняют существующие вопросы и возможности совместной работы.).

Мира и Марк, наряду с представителями других команд, обходят стол и выбирают себе две карточки, относящиеся к облигациям на немецком рынке. В течение двух последних Спринтов их команда обсуждала и детально изучала эти области в ходе внутрикомандных встреч по Уточнению Бэклога Продукта (“PBR”, Product Backlog Refinement).

Ещё они берут две карточки, касающиеся управления заказами, которые обе команды Trade и Margin понимают достаточно хорошо -  они прорабатывали эту тему в ходе совместных встреч по Уточнению Бэклога Продукта. Зачем они делали это вместе? Дело в том, что они хотели определиться с привязкой этой функциональности к конкретной команде максимально поздно, в ходе одного из будущих Планирований Спринта. Это увеличивает гибкость всей группы команд, позволяет легче реагировать на изменения, а также расширяет общие знания по продукту, что улучшает самоорганизацию и общую координацию.

Минуту спустя Мэри из команды Margin, просматривая карточки, отобранные другой командой, спрашивает их представителей: “Вы не будете против, если мы возьмём вот этот отчёт себе? Мы делали нечто очень похожее в последнем Спринте, и я готова поспорить, что мы сможем сделать его быстро. Может быть, обменяем его на вот эту карточку по немецкому рынку?”. На этом они и договорились.

<div>
  {% figure "img/framework/sprint-planning", "Sprint Planning" %}
</div>

Через несколько минут, исходя из своих сильных сторон и интересов, команды определяются с выбором, завершают обмен задачами и концентрируются на задачах группы в целом.

Сэм (Скрам-Мастер) говорит: “Я заметил, что команда Margin выбрала себе четыре задачи, являющиеся наиболее приоритетными. Может ли это обернуться проблемой для нас?”. После небольшой дискуссии участники встречи приходят к тому, что если дела у команды Margin пойдут не так гладко, то есть риск того, что одина из высокоприоритетных задач бэклога може быть не выполнена. Поэтому они решают перераспределить часть высокоприоритетных задач между командами, в соответствии с уровнем их знаний в той или иной области, чтобы увеличить вероятность того, что к концу спринта все высокоприоритетные задачи будут готовы.

В результате встречи участники отобрали 18 карточек, оставив на столе четыре, наименее приоритетные. Паоло проходит взглядом по оставшимся карточкам, берет две из них и говорит: “Эти две задачи важны для меня в этом Спринте. Возможно, мне стоило с самого начала дать им больший приоритет, но я этого не сделал, и сейчас хочу изменить свое решение. Давайте найдем способ поменять их с какими-нибудь из тех, что вы уже выбрали. И, конечно, если какая-то из команд закончит раньше, вы всегда можете взять в работу те, что остались”. 

Когда вопрос с перераспределением решен, Паоло говорит: "Отлично, теперь давайте потратим некоторое время на решение долгоиграющих вопросов. Как вы знаете, до последнего времени я был полностью сфокусирован на уточнениях по более важным задачам, но сейчас предлагаю посмотреть, что мы вместе можем сделать, чтобы подчистить лист менее приоритетных задач.” (ПРАВИЛО: На планировании спринта команды проясняют существующие вопросы и возможности совместной работы).

Параллельно Мира, Марк и остальные формулируют открытые вопросы по своим темам и выписывают их на флипчартах, развешанных по стенам комнаты. Паоло ходит по комнате, от одного к другому, обсуждая неясные моменты с участниками команд. Все слушают и активно помогают дискуссии. Через 30 минут участники закрывают все вопросы, которые не требуют дополнительных уточнений.

Далее участники встают в круг для подведения итогов, но никто не поднимает вопросов, связанных с координацией команд, и Сэм берет инициативу в свои руки: "Я заметил, что команды Trade, Margin и NotDerivative отобрали себе все задачи, относящиеся к теме управления заказами.” Мира восклицает: "О, это же отличный шанс поработать вместе! Давайте тогда организуем общее Второе Планирование Спринта для наших команд.”  Все соглашаются. На этом встреча завершается.

#### Командная и межкомандная Вторая Часть Планирования Спринта

После перерыва две из пяти команд проводят внутрикомандные Вторые Части Планирования Спринта, чтобы сформировать собственные Бэклоги Спринта, а также продумать и распланировать свою работу на ближайший Спринт. (ПРАВИЛО: У каждой команды свой Бэклог Спринта).

Команды Trade, Margin и NotDerivative, наоборот, остаются в большой переговорной для проведения межкомандной Второй Части Планирования Спринта, так как задачи, которыми им предстоит заниматься, тесно связаны друг с другом и уже обсуждались ими ранее, в ходе межкомандного PBR. Команды ожидают получить дополнительную ценность от совместной работы. (ПРАВИЛО: В случае связанных элементов бэклога проводите Межкомандную Вторую Часть Планирования Спринта в общем рабочем пространстве).

Они начинают с десятиминутный сессии, чтобы сформировать общий контекст, понять общие задачи и озвучить потенциальные сложности. Затем они ставят таймер на 30 минут и начинают сессию по проработке дизайна решения, договорившись о визуализации: больше набросков на доске и меньше обсуждений без рисования. За время сессии они находят ещё несколько точек соприкосновения и также выписывают их на доске.

Динь! Отведенные 30 минут завершаются, и многие из деталей все еще остаются непроясненными, но команды решают двигаться дальше. Они расходятся по разным углам комнаты, где проводят индивидуальную Вторую Часть Планирования Спринта, в деталях обсуждая потенциальные сложности с дизайном решения и создавая Бэклогов Спринта на стикерах. Дальнейшая координация между командами происходит посредством продвинутого варианта техники “просто поговорите” (just talk) в LeSS: “просто крикните” (just scream).

В ходе обсуждения участники приходят к пониманию, что необходимо проведения глубокой межкомандной  Сессии по Проектированию Решения (Design Workshop). Они договариваются провести её в тот же день, но чуть позже.

#### Multi-Team Design Workshop

After Sprint Planning and another break, Mira and Mark from Team Trade, and a few people from Team Margin and Team NotDerivative hold a timeboxed one-hour multi-team Design Workshop for a deeper dive into a common and consistent design for their work. Around a large whiteboard they sketch and talk together towards some clarity and agreement on a design approach and common technical tasks. Fortunately, the conclusions don’t seriously impact their existing Sprint plans, but they feel uncomfortable with their process, recognizing they could have predicted the need to resolve these big design questions earlier.

#### Development Activities Supporting Coordination and Continuous Delivery

After Sprint Planning, the teams dive into developing items, with an emphasis on communicating in code. All the teams are integrating continuously. The continuous integration of all code across all teams creates the opportunity to cooperate by checking who else made changes in the component being worked on. That’s useful, because the group uses *integration as a way to inform and support their coordination*.

For example, early during the second day of the Sprint, Mark, a developer on Team Trade, pulls the latest version locally and quickly checks the latest changes related to the component they are working on now. He discovers changes related to code added by Maximilian from Team Margin. He knows that team is working on a strongly related item, so he is not especially surprised. Since the code has communicated that now there’s a need to coordinate and who he needs to talk with, he immediately visits Team Margin down the hall. They just talk about how to work together to benefit from one another’s work. (RULE: Prefer decentralized and informal coordination over centralized coordination.)

For the item that Team Trade is developing, and in fact for every item in every team, they have written the automated acceptance tests before starting to develop the solution code. Thus, in addition to integrating the code continuously, they’re also integrating the automated tests. These acceptance tests are run frequently by team members, and so when any of them fails, the teams are immediately signaled to coordinate. The code is telling them, “Hey! There’s a problem! You need to talk and work it out.”

Naturally, another major benefit of the group’s practice of integrating continuously, automated testing, and stopping-and-fixing whenever the build breaks, is that their product is more or less continuously ready to deliver into production. There’s no separate integration team or testing team that would add delay, handoff, and complexity. (RULE: The perfection goal is to improve the Definition of Done so that it results in a shippable product each Sprint, or even more frequently.)

#### Overall Retrospective

On the second day of the Sprint, Sam and the other Scrum Masters, the Product Owner Paolo, a site manager, and a representative from most of the teams, all get together for a maximum 90-minutes Overall Retrospective related to the *last* Sprint. (RULE: An Overall Retrospective is held after the Team Retrospectives to discuss cross-team and system-wide issues, and to create improvement experiments.)

Why didn’t they hold this Overall Retrospective before this new Sprint started? They could have, but they normally end a Sprint on a Friday and start a new one on Monday (in contrast to Sam’s suggestion that they try a Wednesday–Thursday boundary). And on the last Friday, they held both the Sprint Review and the team-level Retrospectives. After that they didn’t have the energy to hold an engaged Overall Retrospective at the end of the day. So they’ve opted for an early next Sprint. Sam privately thinks this delay is not a great idea—he’d rather they started Sprint Planning a little later after this meeting—but he wants the group to discover that for themselves.

They focus on a system-wide issue and improvement: how to coordinate, share information, and solve problems across the entire group during the Sprint? Previously they have tried Scrum-of-Scrum meetings and didn’t find them very effective. Sam explains the technique of Open Space, and they agree to try it this Sprint.

#### Activities for Coordination

<small>(RULE: Cross-team coordination is decided by the teams.)</small>

The fourth day demonstrates a variety of coordination ideas in LeSS:

In LeSS, each Team holds a Daily Scrum as usual. To support coordination between Teams Trade and Margin, Mira goes as a scout to observe Team Margin’s Daily Scrum and then returns and updates her team on what she learned. And someone from Team Margin does the opposite.

As agreed in the Overall Retrospective, the group holds a 45-minute Open Space meeting for coordination and learning, preceded by drinks and snacks. Sam acts as facilitator to teach the group how to hold an Open Space meeting. Everyone is welcome, but most teams decide to send only a few representatives. Mira and Mark from Team Trade join in. The group plans to try an Open Space once a week.

The Test *community*, with volunteers from most teams, gets together for a half-hour to hear Mary’s proposal to try a new automated acceptance-testing tool. They enthusiastically agree, and Mary volunteers her Team Margin to do the actual experimental work next Sprint, since they are really interested in learning this.

Mira is a member of the Design/Architecture community. There’s no design workshop needed this Sprint related to overall architecture, but she wants to hold a half-day spike in the next Sprint for a new technology. She posts her idea on the community collaboration tool, and suggests the community do the spike together with mob programming to increase their shared learning.

The build system seems to have a weird bug. Time to *stop and fix*! This Sprint, Team Trade is responsible for it, and it’s one of Mark’s secondary specialties, so he volunteers to fix it and asks another team member to pair up with him to help his colleague learn more about it.

Later, Mira and a few other team members visit the customer support and training group, who work closely with hands-on users. Her team has finished their first item and they want to get early feedback from people closer to customers. One of the trainers is free and he plays with the new feature. Team Trade leaves with a few ideas to make it better.

Later in the day Mark and the rest of Team Trade are doing tasks for their second item. Mark has just completed a 10-minute TDD cycle and has clean stable code after a micro-change. Once again—about every 10 minutes—he pushes the tiny change to the central shared repository (to “head of trunk”), to integrate continuously with his team and all others. He glances over to their big visible red-green screen on the wall and sees that the build system is passing all the tests for the entire group.

#### Overall Product Backlog Refinement

<small>(RULE: Do multi-team and/or overall PBR to increase shared understanding and exploiting coordination opportunities when having closely related items or a need for broader input/learning.) </small>

On the fifth day, Mark and Mira join an overall PBR workshop, with representatives from each team, and Paolo, the Product Owner. Paolo starts by sharing his current thinking on product direction and where to go next in the short term and, most importantly, why. To help them understand his reasoning, he reviews his prioritization model with the group, that factors in profit impact, customer impact, business risk, technical risk, cost of delay, and more.

Paolo asks for feedback and ideas from the group for upcoming direction, and the group discusses what items to refine next. Although he knows that he’ll make the final priority calls, Paolo works hard to engage the teams in understanding his thinking, and also to learn from their thinking. He wants the teams to also be involved in owning the product.

The group then splits a few big new items, doing lightweight clarification (more will follow later), and planning poker estimation as a way to learn more about the items—rather than to create estimates.

The representatives from three teams (including Trade and Margin) decide to later do multi-team PBR together for some items to increase their shared understanding and because they are strongly related. And representatives from two other teams choose items to focus on separately in team PBR sessions.

#### Multi-Team PBR and Team PBR

<small>(RULE: All prioritization goes through the Product Owner, but clarification is as much as possible directly between the Teams and customer/users and other stakeholders.)</small>

On the sixth day, everyone in three of the teams gets together for a multi-team PBR workshop in the big room.

Although their main business is creating and selling their trading solution, the company has a small group of bond traders that use it, with relatively small positions that keep them engaged but without high risk. This way the company has better insight into market trends as well as some expert users that can easily talk with the development teams.

Tanya and Ted are the traders who told Paolo about a trend that led to the items being refined in the multi-team PBR session. So they both join, as experts to help the teams learn and clarify the new items.

The other two teams, in discussion with some other traders, hold separate PBR workshops to complete clarification of some items already under refinement and to start on some new ones. Also, one of the company’s three lawyers specializing in financial regulations and compliance joins one of these teams to help them in clarification.

As a last step in the PBR meetings, people take photos of everything on the walls and whiteboards. They add those to the wiki pages that are used to record everything for each item. Plus they update and clean up the text and tables in the wiki pages that were quickly added during discussions.

#### A Chat About Team-Level Backlogs and Product Owners

After the multi-team PBR workshop, Mike (who just joined the company) sees Sam by the coffee machine and walks over to talk. Mike says, “Hey Sam. I’m interested in your opinion on something. In the refinement workshop we just finished, of course I noticed that we were working directly with some of the traders to clarify together. But isn’t that inefficient? In my last company, every team had its own Product Owner who did the story writing, wireframes, and specifications, and then gave them to us to implement. Then we could just focus on the programming. And each team had its own Product Backlog that the team’s Product Owner prioritized. But I don’t see that here. Why is it different?”

Sam says, “Interesting questions. Do you mind if I ask you a few questions to explore this?”

“Sure, go ahead.”

“Let’s first consider one Product Backlog versus many team-level backlogs. Suppose each team had its own backlog. How easy and effective is it for one truly overall Product Owner to have an overview? And how much knowledge will a team have of the requirements and designs of items in a different team’s backlog?”

Mike replies, “I can answer that pretty clearly from my last company. Not much.”

Sam continues. “Now suppose there are eight teams and eight team backlogs. What if, from the higher company or product perspective, for some reason, the items in two of the eight team backlogs are actually by far the most important or highest priority. Maybe there’s some change in the market so that this situation comes up. So some questions for you: Can the six teams working in the lower-priority backlogs easily shift to start working on the high-priority items in the other two backlogs? And is it likely that the group will even see this problem, given that they are locked in to each team having their own backlog and local priorities?”

Mike answers, “Our teams at my old place only worked on their own team item backlog. They couldn’t shift to others. But why would they want to? Isn’t that inefficient?”

Sam responds, “Well, from a company perspective, the teams are only working ‘efficiently’ on low-priority stuff because of their narrow knowledge created by each focusing in a different team backlog and because the overall priority and overview isn’t visible. Let me ask you some questions: Does that seem inflexible or flexible—agile? And does that optimize people working on the highest-impact stuff from the company perspective?”

Mike pauses, “Oh! I think I get it. It’s actually not being agile, even though our group said they were doing agile. We weren’t responsive to the highest-value changes overall. And my old team Product Owner said she was prioritizing for highest value in our team backlog. But now I see that my team was just busy efficiently working on what could be low-value stuff when you look at it from a higher level.” (RULE: There is one Product Owner and one Product Backlog for the complete shippable product.)

Sam says, “Exactly. So that’s one of several reasons why we have one Product Backlog here, and no team backlogs, even though there are many teams. In short, it supports whole-product focus, system optimization, and agility. And of course it’s simpler, and it’s easy to see what’s going on across the group.”

“Also,” Mike comments, “I noticed it was much harder in my prior company for all the teams to really work together at the same time, since we were working on very different goals in asynchronous Sprints. Here it feels like all the teams have more of a common focus and direction in one Sprint together.”

“Exactly!” Sam replies, then continues.

“Here’s another question: If there’s only one Product Backlog and one real Product Owner who prioritizes it, but each team still had its own so-called Product Owner who per definition is not prioritizing a team backlog—since there isn’t one—then what do they do all day long? “

Mike replies, “Well, in my last company it was the job of the team-level Product Owner to talk to the users and write the stories for the team, so they could focus on efficiently programming while the team Product Owner worked on gathering and writing requirements.”

Sam asks, “Mike, before you learned about Scrum terms such as ‘Product Owner’, what would you have called middlemen in between the developers and real customers—the ones collecting requirements and then giving them to developers?”

“I joined my last company before we adopted Scrum there.” Mike answers, “And back in the day, there was a group of business analysts who did that. After we adopted Scrum, we were asked to call them the Product Owners.”

“Today in your PBR workshop,” Sam asks, “Did you talk with the traders who were there?”

“Let me think back.” Mike replies, “Yeah, I was talking with Tanya about her idea to analyze trading Russian corporate bonds. It seemed a little confusing so I asked her, why? She explained it was because of concerns around money laundering in offshore accounts. Now, she didn’t know that we’ve been recently working on some other features that integrate with new EU and USA regulatory databases to assess this. So I proposed to her a different approach, which I think—and she agrees—will better solve the problem.

“Now that I think about it,” he reflects, “that probably wouldn’t have happened in my last company, since we rarely talked directly with users.”

(RULE: The Product Owner shouldn’t work alone on Product Backlog refinement; she is supported by the multiple Teams working directly with customers/users and other stakeholders.)

(RULE: All prioritization goes through the Product Owner, but clarification is as much as possible directly between the Teams and customer/users and other stakeholders.)

#### More Development

Minute by minute and day by day the teams develop code, integrating continuously combined with full test automation. They stop and fix when the build breaks, working towards their perfection goal of having a done shippable product they can continuously deliver to customers. Therefore, when the Sprint is nearly over and the teams are preparing to join the Sprint Review, there’s no late mad rush of effort to integrate and test a big batch of code—it’s been integrated and tested all along.

#### Sprint Review

<small>(RULE: There is one product Sprint Review; it is common for all teams.)</small>

Finally it’s the last day and time for an all-together Sprint Review. Who’s there? Paolo (the Product Owner, lead product manager), all the internal bond traders, a few trainers and customer service representatives, a few people from Sales, and four users from external clients who pay lower annual rates in exchange for participating regularly in these reviews. Also, there’s all the team members.


<div>
  {% figure "img/framework/sprint-review-retrospective", "Sprint Review and Retrospective " %}
</div>

Because there are many items to explore, the group starts with a one-hour bazaar—something like a science fair—with many devices set up in the room, each available for exploring different sets of items. Some team members stay at fixed areas to collect feedback while everyone else uses and discusses the new features.

<div>
  {% figure "img/framework/sprint-review-bazaar-sketch", "Sprint Review Bazaar - Story Sketch" %}
</div>

After an hour, the group comes together to discuss the questions and feedback, in a session led by Paolo. After that, they discuss future direction. Paolo shares what’s going on in the market and with competitors, and his thoughts on where to go next, and asks for advice.

#### Team Retrospectives

<small>(RULE: Each Team has its own Sprint Retrospective.)</small>

After a break, Team Trade (and all other teams) hold separate team-level Sprint Retrospectives. They decide that holding a multi-team Design Workshop with Team Margin after Sprint Planning (rather than earlier) was far from ideal in this case, because major issues were left unexplored until the last minute—issues which could have seriously blocked or complicated development. So for the next Sprint they decide that during their PBR sessions they will strive to identify items that have major design issues worth discussing with other teams. And if so, hold a multi-team Design Workshop as soon as possible.

#### The End

Sprint done! Sam invites Team Trade to join Mira and him at the Belgian-beer pub down the street—Mira’s favorite—to celebrate her birthday. (RULE: Beer is Belgian Tripel Karmeliet.)

#### Summary

Some key points from the story:

* it emphasized flow of people and teams through a Sprint in LeSS
* it connected story elements to specific LeSS guides and rules
* for a reader who knows Scrum, the events should be familiar
* the story shows whole-product focus, even with many teams
* the activities emphasized team-based learning and coordination
* develop items by integrating continuously so that communicating in code supports decentralized coordination and just talking, in addition to continuous delivery
* teams clarify directly with users and customers, to reduce handoff and increase understanding, empathy, and ownership

### • LeSS Story: Flow of Items •

This story focuses more on the flow of items (features) through part of a Sprint, primarily during refinement and development.

Portia wraps up her meeting with the government regulator and heads to the airport, and home. She’s another product manager; she helps Paolo, and specializes in regulatory and audit trends.

<div>
  {% figure "img/framework/product-managers-discuss-sketch", "Product Managers Discuss - Story Sketch", class:"half-sized-figure pull-right" %}
</div>

Later, Portia meets with Paolo. Writing on cards, she summarizes the new rules that are going to impact their product, and what clients she thinks are going to want certain features first. Paolo points to the five cards and asks, “So this covers all the work, as far as you know?” Portia smiles and says, “This is regulatory. It’s never finished or clear.”

Paolo asks, “Can you put these in the Product Backlog for me, unordered at the bottom for now?”

“Sure.”

A week later Paolo tells Portia, “Soon, I want to start delivering some parts of the big regulatory requirement for bond derivatives. In the next Sprint’s Product Backlog refinement workshops, I’m going to ask for some teams to focus on that. You know the most about it, so please be at the overall PBR and at whatever team refinement workshops where they want you. Also, can you set up a wiki page with links to the new regulatory docs, to share with the teams?”

“Already done,” answers Portia.

#### Overall PBR

Paolo kicks off a quick overall PBR workshop, “We’ve got lots of work around new regulations. Soon we need to deliver related items because of a legal deadline end of fiscal year. We’ll know better after some splitting and estimation, but I wouldn’t be surprised if it ultimately involves three or more of the teams for implementation, and lots of time.”

The group splits the new giant item into only a few large parts, to learn major elements. More splitting will happen later in a single-team or multi-team PBR session. Portia heads to the whiteboard; on the left side she writes “regulations for bond derivatives.” Then in conversation with the group, they sketch a tree diagram with four arms representing a splitting into four major sub-items. But they don’t go any deeper—they’re avoiding over-analysis.

Next, the group creates four cards for the new items, and everyone together estimates them with planning poker and relative-size points, baselining the points against existing well-known items in the Product Backlog. Their main goal is not to create estimates but to surface questions and drive more discussion, which they do with Portia.

Next, Paolo asks, “So Portia, of these four big ones, which one first?”

She points to the second card. “Over-the-counter exotic bond derivatives.”

Paolo says, “We need to start delivering some of that as soon as possible. It’s moving way up the Product Backlog. So I’d like one team to take a bite into this, next Sprint. Who’s interested?”

Team Trade volunteers.

Finally, team members from three other teams decide to hold a multi-team PBR workshop for related items.

#### Team PBR: Biting In

The next day Team Trade holds a team PBR workshop with Portia. They have only one of the four giant items to focus on: New regulations for over-the-counter (OTC) exotic bond derivatives. Sam (their Scrum Master) is also there. Portia says, “This is a gigantic complex item, in an area that frankly nobody is really clear about. It’s going to take us a long time to split this up, really understand it, and specify it well.”

Sam asks, “Do we really need to understand all of it? And will all that analysis teach us more, or could it actually delay our learning?”

He reviews with them the idea of Take a Bite: to just split off one tiny fragment, really understand that, and implement it quickly. Sam concludes, “You know, diagrams don’t crash and documents don’t run.”

With Portia, the team splits off one tiny bite of a thin customer-centric end-to-end item.

From now on they will focus on that tiny bite, clarifying and implementing it. Only after implementation and feedback will they return much later to more splitting and refinement. Using specification by example Portia and Team Trade spend the rest of the day chewing on their bite.

#### Multi-Team PBR: Rotation Refinement

One outcome of overall PBR was the decision to take a bite with Team Trade. Another was the decision for three teams to hold a multi-team PBR workshop for related items, to increase learning and the agility of multiple teams knowing and thinking about the same items.

In addition to everyone from the three teams, the internal traders Tanya, Ted, and Travis join to help the teams start clarifying about a dozen new items. (RULE: All prioritization goes through the Product Owner, but clarification is as much as possible directly between the Teams and customer/users and other stakeholders.)

To start, they form three temporary mixed groups with people from each team. The mixed groups start clarifying different items in separate areas in the room, each with a whiteboard, big wall space, laptop, and projector. Tanya is with one group, Ted another, and Travis, the third.

Then they do rotation refinement: After 30 minutes, a timer goes ding! One group walks over to the other’s area, and vice versa, but Tanya, Ted, and Travis don’t move. The timer is restarted, the traders explain the current results to the incoming groups, and they continue clarifying.

<div>
  {% figure "img/framework/multi-team-product-backlog-refinement-sketch", "Multi-Team Product Backlog Refinement - Story Sketch" %}
</div>

Throughout the day, as different items become relatively clear—or are left with hanging questions that will have to be explored later—new items are introduced at a work area. Some of the bigger items are split into two or three new smaller ones.

A few times during the day, the groups stop their clarification and do some estimation, mostly to learn and to prompt conversation. They’re using relative (story) points; to remain synchronized against a common baseline, they calibrate against some already completed and well-known items in the Product Backlog.

#### Updating the Product Backlog and Product Owner

The day after the PBR workshops, Portia and a few team members

* update the Product Backlog with the new split items derived from the original ones, and delete the originals
* add links to the new wiki pages of item details, created in the PBR workshops
* record new estimates, and items ready for implementation

Later, Portia and those team members meet with Paolo to review the Product Backlog changes and to answer his questions.

#### The End

Some key points from the story:

* Take a Bite on a giant item to learn from delivery of something small and to avoid premature and excessive analysis.
* Do multi-team PBR for items, for shared knowledge across teams, which increases organizational agility, broadens whole-product knowledge, and fosters self-organized coordination.
* Strive for whole-product focus, even with many teams.

**Next**—The next section shifts to the *LeSS Huge* framework, used for large groups of many teams.

## LeSS Huge Framework

### • Requirement Areas •

With 1000 or even just 100 people on one product, divide-and-conquer seems unavoidable because of the complexity of so many requirements and people. Traditional large-scale development divides these ways:

* single-function groups (analysis group, test group, …)
* architectural-component groups (UI-layer group, server-side group, data-access component group, …)

This organizational design yields slow inflexible development with (1) high levels of waste (inventory, work-in-progress, handoff, information scatter, …), (2) long-delayed ROI, (3) complex planning and coordination, (4) more overhead management, and (5) weak feedback and learning. And it is organized *inward* around single-skills, architecture, and management, rather than outward around customer value.

But in the **LeSS Huge** framework when above about [eight](#the-magic-number-eight) teams, division is around *major areas of customer concerns* called Requirement Areas. This reflects the *customer-centric* [LeSS principle](#less-principles-).

**Size**—A Requirement Area is *big*, usually with between *four and eight teams*, not one or two. The following Area Feature Teams section explains why.

**Dynamic**—Requirement Areas are dynamic. Over time an area will change in importance, and then it grows or shrinks with teams joining or departing—most likely to or from another existing area.

**Example**—For example, in a Securities product (to trade stocks), these could be some major areas of customer interest—Requirement Areas:

* trade processing (from pricing to capture to settlement)
* asset servicing (e.g. handling a stock split, dividends)
* new market onboarding (e.g. Nigeria)

Conceptually in the one Product Backlog, a Requirement Area attribute is added, and each item is classified into one and only one area:

| Item   | Requirement Area      |
|:------:|:---------------------:|
| B      | market onboarding     |
| C      | trade processing      |
| D      | asset servicing       |
| F      | market onboarding     |
| ...      |
{: .grid_table_with_header}

Then people can focus on one Area Product Backlog (conceptually, a view onto one Product Backlog), such as the *market onboarding* area:

| Item   | Requirement Area     |
|:------:|:--------------------:|
| B      | market onboarding     |
| F      | market onboarding     |
{: .grid_table_with_header}

**Common Sprint**—Does each Requirement Area work separately in its own Sprint, with delayed integration until a far-future date? No.

*In LeSS Huge, Integrate Continuously in One Common Sprint*
There is one product-level Sprint, not a different Sprint for each Requirement Area. It ends in one integrated whole product, and all the teams across all the Requirement Areas are striving to integrate continuously across the entire product.
{: .box_top_bottom .text_centered_bold }

### • Area Product Owners •

In LeSS Huge one new role is introduced. Each Requirement Area has an Area Product Owner who specializes in that area and focuses on its Area Product Backlog.

Large product groups usually have several supporting product managers specializing in different customer areas, and some of these are likely to serve as the Area Product Owners. Sometimes the Product Owner also serves double duty as an Area Product Owner for one area; that’s more likely in small *less huge* LeSS Huge groups!

### • Area Feature Teams •

Area feature teams work within one Requirement Area (e.g. asset servicing), with one Area Product Owner focusing on the items in one Area Product Backlog. From a team’s perspective, *working in the area is like working in the smaller LeSS framework*—they interact with their Area Product Owner as though she were the Product Owner, and so on.

The team members come to know the customer domain of that area well. And fortunately, the items of one Requirement Area tend to cover a semi-predictable subset of the entire code base, thereby reducing the scope of what they have to learn well within a vast product.

Key point about size: *Many* feature teams work in a Requirement Area.

A Requirement Area normally has four to eight teams.
An implication is that a Requirement Area is big.
{: .box_top_bottom .text_centered_bold }

#### The Magic Number Four

First, why does a Requirement Area have a suggested upper limit of eight teams? See [The Magic Number Eight](#the-magic-number-eight).

What about the lower limit of four teams? Why not one or two teams? Naturally, four isn’t a magic number, but it strikes a balance so that the product group is not composed of many tiny Requirement Areas.

What’s the problem with many tiny areas? They reduce visibility into overall product-level priorities, increase local optimizations, increase coordination complexity, require more positions, and create teams that are too narrowly specialized and lack the flexibility (agility) to take on the emerging highest-value items from a company perspective. Furthermore, in a tiny area the Area Product Owner is increasingly likely to act as a business analyst between the users and one or two teams.

Are there any reasonable *exceptions* to the lower limit of four? Yes:

* An early transitional situation when the group is incrementally growing a new area that is fully expected to ultimately have four or more teams. Then, start small and simple with one team.
* When re-balancing teams from an area with a decreasing demand to one with an increasing demand causes an area to go from four to three teams. Ultimately, merge two reduced small areas back into a new larger area.

#### Example Requirement Areas and Teams

In summary, a Securities product could have

* one Product Owner and three Area Product Owners, all together forming the Product Owner Team
* six feature teams in the trade processing area
* four feature teams in the market onboarding area
* four feature teams in the asset servicing area

### • LeSS Huge Framework Summary •

<div>
  {% figure "img/less-huge/less-huge-framework", "LeSS Huge Framework" %}
</div>

Each Requirement Area works as a (smaller framework) LeSS implementation, each working in parallel in one overall Sprint. We sometimes summarize a Sprint in LeSS Huge as a *stack* of LeSS.

From the viewpoint of a team in one area,
LeSS Huge looks like (smaller) LeSS regarding events.
{: .box_top_bottom .text_centered_bold }

As with LeSS, there are [rules](https://less.works/less/rules/index.html) and optional **guides** for LeSS Huge; those are introduced in the following stories and fleshed out in later chapters.

**Roles**—Same as LeSS, plus two or more Area Product Owners, and four to eight Teams in each Requirement Area. The *one* Product Owner (who focuses on overall product optimization) and the several Area Product Owners form the Product Owner Team.

**Artifacts**—Same as LeSS, plus a *Requirement Area* attribute in the one Product Backlog and thus an Area Product Backlog view for each area.

**Events**—There is still only one common Sprint for the product; it includes all the teams and ends in a common potentially shippable product increment.

### • LeSS Huge Stories •

**Learning LeSS Huge**—Readers who prefer exposition can comfortably skip ahead to following chapters, bypassing these stories.

**Simple stories**—These are intentionally plain and simple stories just to introduce basics in LeSS Huge.

**Two topics**—Following are two stories with distinct topics:

1. [Creating and growing a new Requirement Area to deal with a new gigantic requirement.](#less-huge-story-a-new-requirement-area-)
2. [Working with multi-site teams. (This happens in the smaller LeSS framework too, but is especially common in LeSS Huge.)](#less-huge-story-multi-site-teams-)

### • LeSS Huge Story: A New Requirement Area •

Priti welcomes Portia to her first day in her new job. As a mid-level Operations manager in the Securities division of the large trading company as well as Product Owner for their internal Securities system, Priti is also responsible for finding and retaining talent for her Product Owner Team of Area Product Owners. And she thinks Portia is a fantastic find, as her expertise is exactly what is required for dealing with some new huge requirements.

During the recent job interview—when Portia was still a product manager specializing in regulatory issues at a company that made a system for trading bonds—Priti had laid out the situation. “Portia, after the last crash, the regulators are coming down hard and they require us to be compliant with Dodd-Frank. Right now, we don’t know what it exactly means or how it will impact our system. You’ve got incredible knowledge of this space, and a great professional network with the regulators. I would love it if you would join our group and help us figure out how to deal with this.”

#### A Big Surprise

A few days later… Priti welcomes Portia, Peter, and Susan into her office. Peter is Area Product Owner for market onboarding, and Susan is a Scrum Master from the trade processing area.

Priti says, “As you know, Dodd-Frank is coming, and it’s huge. What you don’t know is that this morning the regulators called us and they want us to take action now. I’d been working under the assumption we could start next year. So we’re going to have to adapt, big time.

“I don’t think anyone is clear what it means in detail—even the regulators. And we don’t know how it will impact our system and how much work this is going to take, other than, a lot! But now Portia’s joined us and she has a better understanding of this than anyone, although she’s totally new to our systems. So, how can we help her start tackling this mountain of work?”

Susan asks, “You guys understand the Dyslexic Zombies, right?”

Peter and Priti nod. Everyone knows about them—and it isn’t just their name. The Dyslexic Zombies have probably the broadest experience of all the teams. They’ve been around for years and they were a true pain in the ass when they adopted LeSS. The team contained two former members of their now-abandoned architecture group and a couple of people who had been working on the system for over fifteen years. Those people’s resistance to the LeSS adoption was legendary as they were afraid they’d lose their “system perspective.” To their surprise, the opposite happened! Because of their deep knowledge they continuously get tough items to develop. And they regularly participate as expert-teachers in current-architecture-learning workshops with newcomers, and Mario—one of the former PowerPoint architects—is now coordinator for the architecture community. When fed enough beer, he’ll admit that working closer with code and tests has increased his real understanding of the system.

<figure>
  <img src="/img/framework/zombies.png" alt="zombies.png" class="half-sized-figure pull-right">
</figure>
Susan continues, “If any team can quickly help Portia get a better understanding of the size and impact of Dodd-Frank, it’ll be the Zombies. And they led the work on Sarbanes-Oxley a few years ago. Tomorrow is their PBR session. They are just about wrapped up on a new feature. Why don’t we re-direct the meeting to include them in a discussion on Dodd-Frank, and soon after, ask them to focus full-time on it?”

#### Refining with Zombies

Next day at the refinement meeting with the Zombies, Portia explains the situation, “You’ve probably all heard about the Dodd-Frank legislation. But here’s the surprise: We’ve just been told by the regulators that they want us to take action ‘now’ and demonstrate significant compliance by the end of the year. Otherwise they might restrict our trading.”

The Zombies are visibly surprised. They had heard rumors but didn’t expect such a rush!

Mario says, “OK Portia, give us a quick summary of what this means. And how is it different from Sarbanes-Oxley?”

<div>
  {% figure "img/framework/splitting-at-whiteboard-sketch", "Splitting at Whiteboard - Story Sketch",
  class:"half-sized-figure pull-right" %}
</div>

Portia picks up a pen and starts sketching on a whiteboard. After about 45 minutes, she is finished with the overview and the Zombies looked a little stunned.

“End of the year, they said?” says Mario. “If the whole group started today, it wouldn’t get finished. This is huge!”

He takes a pen and at the whiteboard starts a rough sketch of their system, talking with the other Zombies about the impact it might have.

He says, “Portia, let’s also use this as a chance to help you understand the system better. Ask away.”

Portia says, “Can you hold on for a second? Let me start a video recording to help me remember this.”

Michelle, a veteran in the team, says, “We’d better start on some real development soon and learn more as we go because otherwise we’ll end up analyzing forever. I’ve seen this story before.”

Susan, their Scrum Master, says, “Reminds me… Tom DeMarco once said that the reason for every failed project is that it started too late.” Everyone laughs. She continues, “So here’s a suggestion: take a bite.”

#### Creating a New Requirement Area

The next day, Portia, Priti, and rest of the Product Owner Team meet. Portia shares a summary of the scope as she understands it now.

Priti says, “This is even bigger than I expected, and we need to show some tangible progress to the regulators within a few months, and major progress before fiscal year end—seven months from now. To state the obvious, they’re now authorized to require more from us, and with the power to shut us down. As you know, just last month the CEO made it crystal clear that new regulatory requests take priority over any other concern. It’s my experience that our goodwill and flexibility with the regulators goes up if we can give them something early, and be transparent and responsive. So that’s what we’re going to do.”

Priti continues, “It seems to me that we’ll need a new area for this big surprise. And of course that’s probably going to impact some of our existing high-priority goals, since we’ll have to shift some teams. Let’s prepare for a deeper discussion of overall prioritization impact in a couple of days. But for now, I’d like your input about spinning up a new area.”

After a short discussion, it’s clear that everyone recognizes the importance of creating a new area.

Priti then says, “Portia, I know you are new to us, but do you think you would be able to handle the Area Product Owner responsibility for this?”

Portia nods.

Priti continues, “Peter, do you think the Zombies could start work on this? And we’ll need them to learn more Dodd-Frank and figure out the impact on our system before we can add more teams to this.”

Peter says, “I don’t think we’ve got any choice.”

Priti says, “OK Portia, so currently we’ve got a few items in Peter’s Area Backlog, the one huge item I think you called “remainder of Dodd-Frank” and the tiny item which the Zombies and you split off of it. Please ask Peter to show you how to set up a new area in the Product Backlog and move the items over to it.”

Priti continues addressing the group, “The next Sprint starts in three days. Let’s move the Zombies into your area and get started on this monster. Probably in a couple of Sprints we’ll be ready to—and need to—grow your area by moving in another team. Folks, please think about two major concerns: First, preparing for a serious prioritization impact meeting in a few days. And second, what other teams will be good candidates for the new area.”

#### Sprint Planning in the New Requirement Area

Each Requirement Area holds its own Sprint Planning meetings, all more or less in parallel. In Portia’s new area, she starts her Sprint Planning by introducing two unfamiliar faces to the Zombies.

She says, “Gillian and Zak have been in contact with the regulators regularly and will help us flesh this thing out. They’ve agreed to help us now in Planning, during our PBR sessions, and as much as they can spare daily during upcoming Sprints.”

She continues, “Here’s my tentative plan of attack for the next two Sprints. First, together we need to learn more about Dodd-Frank, and also split it into some major and manageable pieces so we can start to clear the fog and get a better sense of priorities.

“Second, we implement the smaller bite we’ve taken, starting this Sprint. That’ll give us better information about the real work and the impact on our product. And we’ll have some concrete visible progress.

“Third, we prepare for more teams to join our area. What do you think of this approach? Other suggestions?”

During the short discussion, Mario says to his team, “Let me give a bit more context, because I represented our team in the recent Product Owner Team meeting with all the Area Product Owners and Priti. To start with, it’s just us to start. We’re going to take the lead on early implementation, and getting the big picture of the item, and understanding the overall impact on our architecture.”

Michelle interrupts, “Like a tiger team working on a new product?”

“Yes, like that,” says Mario. “Think of Dodd-Frank support as a new product that needs to be continuously integrated into the rest of the product. But we’re in a hurry and it’s a ton of work, so in a few Sprints one more team will join us and shortly after, probably two more teams. We keep developing too, but we’ll be the leading team, which means we’ll need to bring the other teams up to speed and make sure we keep the overall product in mind.”

Michelle says, “It’s starting to sound to me like we’re going to become the architecture and project management team!”

Mario laughs, “No. I’m done with that. We’re still a normal feature team, but besides development we’ll focus on mentoring and bringing the new teams up to speed as fast as possible. But let’s be clear: team coordination and management is still the responsibility of each team.”

#### The First Sprint in the New Requirement Area

Their first Sprint is an unusual balance of clarification versus development, but nevertheless quite useful in this extreme situation. They spend almost half the Sprint in clarification with Portia, Gillian, and Zak. That’s because even for this extremely small bite, trying to understand what is wanted in the obscure realm of new government regulations—with no direct access to the politicians and policy writers—required a lot of investigation, reading, discussion, and communicating with outsiders. They expect that in future Sprints, the amount of time needed for clarification will soon drop down to a more common 10% or 15% of their Sprint.

And so they also only spend about half the Sprint developing one small item. But the discussion and the learning from coding pays off. Slowly but surely they start to split Dodd-Frank apart—at least the parts that any of them can understand.

While implementing the small item they had bitten off first, they spend much of the time together at whiteboards to discuss the overall design implications on the system. The team moves frequently back and forth between the code and the wall.

#### Sprint Review in the New Requirement Area

The overall Securities product group works together in one Sprint, with one final shippable product increment. But each Requirement Area holds its own Sprint Review, all more or less in parallel.

In Portia’s area, during their Review, she, Gillian, and Zak explore the one “done” item that the Zombies have managed to complete and integrate into the overall product. They had originally forecast two items, but Portia is impressed that they got even one done, given how fast this new work was thrown at them.

#### The Second Sprint

In the second Sprint they’re able to make slightly better progress on items, though they once again spend a lot of time clarifying together with Portia, Gillian, and Zak.

In the middle of the Sprint they hold a multi-team PBR session with the second team that is planned to soon join the area, teaching them about Dodd-Frank. They hold a current-architecture learning workshop to introduce the team to the major design elements already in place.

The Zombies know how big the work is and look forward to more help.

#### Product Owner Team Meeting

A few Sprints later… It’s time once more for the per-Sprint Product Owner Team meeting. They use it to align and coordinate between the different Area Product Owners, and for Priti to give guidance.

The Area Product Owners each share in turn their situation and upcoming goals. When it’s her turn, Portia says, “To none of our surprise, the progress is little and the surprises are big. But the fog is clearing and the teams and I are getting our heads around the work. Gillian and Zak have been tremendous help.”

Pablo, the Area Product Owner of asset servicing, comments on some close item relationships he now sees between their areas. Portia agrees to meet with Pablo and some team representatives later.

Priti asks, “Portia, about our upcoming Sprint. What are your goals?”

#### Adding a Third Team

Two Sprints later… At the Product Owner Team coordination meeting, Priti says, “As you know, Portia’s area still has only two teams. I know that Pablo would like to keep his six teams in asset servicing, but Dodd-Frank is just too important to me this year. So we’re going to move one team from Pablo’s area into Portia’s. Pablo, please ask for a volunteer team from your group and let me and Portia know.”

#### The End

Some key points from the story in LeSS Huge:

* The Product Owner is responsible for finding Area Product Owners and developing their talents.
* The Product Owner is responsible for deciding to start, grow, or wind down Requirement Areas.
* Requirement Areas are large, normally requiring four to eight teams, but during initial startup they may be smaller, especially if initiated with one team using a Take a Bite approach.
* A Leading Team works solo to tackle a gigantic item until they understand the domain and development, and then they coach more incoming teams to help with the vast work.

### • Multi-Site Teams: Terms & Tips •

Next is a LeSS Huge story involving multi-site teams. But first, some clarifying definitions, because the common term distributed teams confusingly means several things. The clarifying terms are as follows:

* **dispersed team**—One team of (e.g. seven) people spread out in different locations; either different rooms, buildings, or cities
* **co-located team**—One team working literally at the same table
* **multi-site teams**—One co-located team working at one site, and another co-located team working at another site

Second, an observation and guidance:

* A dispersed team is rarely a real team; it is much more likely a loosely connected groups of individuals. The communication and coordination frictions are higher, and they seldom jell as a team.
* When your product group is 50 or 500 people, dispersed teams aren’t necessary. Each team of seven-ish people can easily be co-located. However, some teams may be in different sites, so that the product group has multi-site teams. Dispersed teams are usually the result of bad organizational decisions and ignorance about the cost of not having co-located teams. (Rule: Each team is (1) self-managing, (2) cross-functional, (3) co-located, and (4) long-lived.)

### • LeSS Huge Story: Multi-Site Teams •

Portia is the Area Product Owner for a new Requirement Area in a Securities trading system. The new area started with just one team for focus and simplicity. A few Sprints later Portia’s area adds a third team. Her first two teams are based in London with her. But her third new team, HouseDraculesti, is based in Cluj Romania at a major development site for the company.

Why not add a third team from the London site? That would have avoided the many aggravations and efficiency penalties that can come from multi-site development within one area—costs potentially so high that adding a team can effectively result in deleting a team.

But on the positive side in this case, Cluj is only two time zones from London, and everyone there speaks English well. And they are all strong developers with Computer Science degrees, in a city that values long-term and hands-on engineering mastery. Also, this is a dedicated internal development site for the company, so these are experienced internal teams that have in-depth knowledge of the product and domain.

And bottom line, Priti (the Product Owner) didn’t want any of the other London teams to shift from their current areas.

Priti knows that multi-site teams are a new situation for Portia, and so at their next meeting, she says, “Please ask your Scrum Master to talk with Sita, and also ask Sita to coach some of your events. She’s a Scrum Master in asset servicing, and she’s observed their multi-site situation for a few years. She knows the importance of Scrum Masters co-located with their teams, and she’s helped facilitate many multi-site meetings.”

Priti continued, “Also, we’ve had a super profitable year, so I’m providing funding for you and the Zombies team—at least those that can travel—to spend a Sprint in Cluj as soon as possible. Work closely with them, all in one room. The Cluj team could come here to London, but you want to send a strong signal that they are important, at their site. Try to avoid making them feel that London is more important than Cluj. Oh—and you’ll want to regularly visit every few months.”

#### Multi-Site Sprint Planning Part One

A few Sprints later, Portia walks into the room. There’s a computer projector attached to a laptop, displaying via video a room in Cluj. The whole team in Cluj are sitting and waiting. Sita suggested it would improve learning and engagement if the entire Cluj team participated in multi-site meetings for the first few months of their addition to the area.

All the team representatives have tablets or laptops with them.

Portia begins. “Welcome and let’s get started. My offer of items this Sprint are highlighted in the shared spreadsheet. Can you all see it? I think you all understand why these are the themes and priorities, since we’ve been discussing this in PBR and it reflects your input and mine. But please ask again if you’d like clarification. Other than that, you’re invited to enter your team names beside the items you want.”

That done, the group enters a Q&A phase to wrap up lingering questions about the items. The London representatives tape up some flip-chart papers and start writing questions. The Cluj team members enter their questions in separate sheets of a shared spreadsheet. Portia spends some time at the different paper flip charts, discussing answers and sketching on the paper. And she spends some time at the spreadsheet, typing in answers for the Cluj team, while also talking with them face-to-face via the video session.

After about 30 minutes the separate questions have been resolved, and Portia asks everyone to come back together. She says, “Any issues or questions that you want to discuss together, before we wrap up?”

#### Multi-Site Overall PBR

People enter the workshop room in London for multi-site PBR. Two projectors are set up. One shows a video session of the workshop room in Cluj. The other displays a browser on Portia’s computer.

Portia says, “Let’s get started. I want to focus on splitting some items. I’ve invited Zak to join us because he knows quite a lot about this.”

Using a mind-mapping, browser-based graphics tool, Zak starts to create some branches, while discussing with the group.

<div>
  {% figure "img/framework/multi-site-estimation-with-planning-poker-sketch", "Multi-site Estimation with Planning Poker",class:"half-sized-figure pull-right" %}
</div>

Afterwards, they use a shared spreadsheet to discuss and write a single example for each of the new split items, so that the people at both sites gain a lightweight but concrete understanding of the details. Later, the group does estimation of the new items, using especially big planning poker cards that can be easily seen by the cameras and video when held up.

#### The End

Some key points from the multi-site story in LeSS Huge:

* Multi-site teams frequently create both obvious and subtle frictions and costs that are surprisingly large in their negative impact.
* Qualities that reduce the friction of another site include similar time zone, internal dedicated site (not outsourced), developers that are fluent in the same spoken language, a location and culture that highly values long-term hands-on developer excellence.
* A Scrum Master must be co-located with their teams.
* Each site must feel like a peer, not a second-class citizen.
* Sites must be visited regularly and cross-pollinated.
* In meetings, strive for face-to-face with video tools.
* The use of shared-document tools make it easy for everyone to modify artifacts together and at the same time.

### Onwards

Rather than asking, “How can we *do agile* at scale in our complex and awkward organization?”, ask a different and deeper question, “*How can we simplify the organization*, and **be agile** rather than do agile?” And since truly scaling Scrum starts with changing the organization rather than changing Scrum, the next major section focuses on understanding and adopting a simpler customer-focused LeSS *organization*.

This is followed by major sections on a more customer-focused product and Sprint in a simpler LeSS organization.