---
title: Specification by Example
order: 70
---

<div class="chapter_quote"><p>
Two things are infinite: the universe and human stupidity; and I’m not sure about the universe.
<br/>
--Albert Einstein
</p></div>

Specification by Example or Acceptance test-driven development (A-TDD) is a collaborative requirements discovery approach where examples and automatable tests are used for specifying requirements—creating executable specifications. These are created with the team, Product Owner, and other stakeholders in requirements workshops.

Note on terminology: We'll use both A-TDD and Specification by Example

A-TDD integrates some major ideas:

* tests as requirements, requirements as tests
* workshops for clarifying requirements
* concurrent engineering
* prevention instead of detection

**Tests as requirements, requirements as tests**—In [Exploring Requirements: Quality before Design](http://www.amazon.com/Exploring-Requirements-Quality-Before-Design/dp/0932633137), authors Gause and Weinberg investigate the link between requirements and tests, “one of the most effective ways of testing requirements is with test cases very much like those for testing the completed system”. [Melnik and Martin](http://gmelnik.com/papers/Melnik-Martin-Tests-and-Requirements-The-Moebius-Strip-IEEE-Software-2008.pdf) extend this further and claim, “As formality increases, tests and requirements become indistinguishable. At the limit, tests and requirements are equivalent”. Tests must be precise in order to be automatable. A-TDD exploits this formality and formulates requirements by writing automatable tests.

**Workshops for clarifying requirements**—The sixth agile principle reminds us “The most efficient and effective method of conveying information to and within a development team is face-to-face conversation.” Face-to-face requirement clarifications in workshops have been used since the invention of [Joint Application Design (JAD)](http://www.amazon.com/Joint-Application-Development-Jane-Wood/dp/0471042994). And these are also used in [Rapid Application Development (RAD)](http://www.amazon.com/Rapid-Application-Development-James-Martin/dp/0023767758) and the agile method [DSDM](http://www.amazon.com/DSDM-Dynamic-Systems-Development-Practice/dp/0201178893). A-TDD similarly exploits face-to-face conversation by using workshops for formulating requirements-as-tests.

**Concurrent engineering**—The authors of [Concurrent Engineering Effectiveness](http://www.amazon.com/Concurrent-Engineering-Effectiveness-Integrating-Organizations/dp/1569902313) define concurrent engineering as follows: “There is a tight link between participants in the product development process, such that they can perform much of their work at about the same time.” The main driver of concurrent engineering is shorter cycle times in development. Two-week iterations are fast and therefore the team needs to conceive a way to work concurrently—sequential development in a short iteration does not work. We have seen teams invent Specification By Example again and again simply because they had to answer the question: “How can we perform our work at the same time.”

**Prevention rather than detection**—In one of the first studies of Toyota, [A Study of the Toyota Production System](http://www.amazon.com/Study-Toyota-Production-System-Engineering/dp/0915299178), Singeo Shingo writes “The purpose of inspection must be prevention; however, for inspection to have that function, we must change our way of thinking.” Similarly, in [“The Growth of Software Testing,”](http://www.clearspecs.com/downloads/ClearSpecs16V01_GrowthOfSoftwareTest.pdf) the authors identify five periods in the evolution of software testing. They call the latest period “The prevention-oriented Period” and state, “Asking test-related questions… early is often more important to software quality and cost-effective development than actually executing the tests.” This is exactly what Specification by Example strives to do. When including people specialized in testing in the requirements workshop, they can ask the test-related questions, and in that way improve the requirements and prevent defects. The Total Quality movement—an influence to Toyota and lean development—also promotes prevention over detection.

How does A-TDD work? The below figure presents an overview.

<figure>
  <img src="/img/test_automation/atdd.png" alt="atdd.png">
  <figcaption>A-TDD Overview</figcaption>
</figure>

## A-TDD overview

A-TDD consists of three steps:

1. Discuss the requirements in a workshop.
2. Develop them concurrently during the iteration.
3. Deliver the results to the stakeholders for acceptance.

**Discuss**—Requirements are discovered through discussion in a requirements workshop. Participants of a workshop are the cross-functional team, the Product Owner or representative, and any other stakeholder who potentially has information about the requirements. A common question to ask during such workshops is “Imagine the system to be finished. How would you use it and what would you expect from it?” Such a question results in examples of use, and these examples can be written as tests—the requirements. The workshop focus ought to be on discussion and discovery of requirements more than on the actual tests.

**Develop**—At the end of the workshop, the examples are distilled into tests and all activities needed to implement the requirement are done concurrently. These include:

* making the glue code between the tests and the system under test (“test libraries” and “lower-level tables” in Robot Framework or ‘fixtures’ in Fit)
* implementing the requirement so that the tests pass
* updating architectural and other internal documentation according to the working agreement of the team
* writing customer documentation for the requirement
* additional exploratory testing

The exact list depends on the product, context, working agreements, and the [Definition of Done](../framework/definition-of-done.html).

**Deliver**—When the tests pass, the requirement is reviewed with the Product Owner and other stakeholders. This might lead to new requirements or a change in the existing tests.

A more detailed way of describing A-TDD is shown below

<figure>
  <img src="/img/test_automation/atdd_clarified.png" alt="atdd_clarified.png">
  <figcaption>A-TDD in more detail</figcaption>
</figure>

The steps in A-TDD map nicely to the LeSS cycle

<figure>
  <img src="/img/test_automation/atdd_in_iteration.png" alt="atdd_in_iteration.png">
  <figcaption>A-TDD steps mapped to Scrum iteration</figcaption>
</figure>

*Discuss in workshop*—Before the detailed Sprint Planning, the team, Product Owner, and other stakeholders clarify the requirements collaboratively in a workshop.

*Develop in concurrence*—Tasks for implementing the tests/requirements are created in the detailed Sprint Planning and implemented during the iteration. All activities happen “at about the same time.”

*Deliver for acceptance* —The working product increment—the passing acceptance tests—are delivered for acceptance to stakeholders and discussed together in the Sprint Review.

## Discuss in Workshop

The workshop-related experiments are strongly connected to those in the Requirements chapter. This section covers A-TDD-oriented topics; the Requirements chapter covers requirements workshops in more detail.

### Discuss in workshop during Product Backlog refinement

The team and Product Owner ‘inspect’ the Product Backlog during the [Product Backlog refinement](../framework/product-backlog-refinement.html) to ensure it is in a good shape. This activity includes the following:

* Estimate and clarify newly added Product Backlog items.
* Split large items into smaller ones so that they can be selected for implementation.
* Clarify the imminent items so that the team understands them well enough to implement them.

The clarification of imminent items can be done through A-TDD-style requirements workshops. Just to be clear, Product Backlog refinement is not only a A-TDD requirement workshops, but it can be part of the refinement activity. Other activities include estimation and splitting.

### Clarification over writing tests

A-TDD is for collaboratively clarifying requirements. The emphasis is on communication, collaboration, and learning through examples and tests. The goal is increased understanding, and tests are the means of getting there. The appropriately titled book on this subject, [Bridging the Communication Gap](http://www.amazon.com/Bridging-Communication-Gap-Specification-Acceptance/dp/0955683610) stresses:

> [Acceptance-test driven development] is not a programming technique: it is a communication technique that brings people involved in a software project closer.

People are often so preoccupied with the tangible outputs of a workshop—the tests—that they forget about the intangible outcomes—the learning. Understanding and clarity of the requirements is the key output of a requirements workshop; the tests are an expression of these.

This is not a false dichotomy. The tests are important, and this technique is called acceptance-test-driven development. Without tests, it would be just a requirements workshop—but avoid confusing means with ends.

### Use examples

> “Can you give me an example?”

This question can suddenly transform a vague and abstract discussion into a clear and concrete one. When discussing new products, people tend to end up talking in concepts and abstract terms. They talk past each other without understanding—they are stuck. Asking for examples brings the discussion back to reality.

For example, we hear assertions such as “The system needs to recover from error situations.” This is vague, so we ask for examples that transform the discussion. This could be “When we unplug the cable, the system should not crash”—which is concrete and understandable. Examples are also used for further clarification, such as, “How should the system recover if we remove a unit from the system while it is running?”

Examples are not just useful for clarifying requirements, but also for clarifying ways of working. “We could never automate all our tests!” is something we would follow up with “Can you give me an example of a non-automatable test?” and that moves the discussion away from principle and into practice.

<figure>
  <img src="/img/test_automation/examples.png" alt="examples.png">
  <figcaption>Examples</figcaption>
</figure>

The above figure shows the relationship between examples, requirements, and tests. During requirement workshops, use examples to elaborate requirements and transform these into tests.

### Don't ‘optimizing’ the requirements workshop

When we were discussing A-TDD with a large product group, they noted, “We improved the A-TDD workshop. Only three people participate: the Product Owner, the Scrum Master, and a specialist in the team.” We asked them how the other team members would understand the requirements so that they can implement them and the answer was, “The specialist will tell them.” They ‘optimized’ the workshop by reintroducing traditional analyst-team handoff.

### Avoid using computers and projectors in the workshop

Computers suck the lifeblood out of a workshop. They become the center of the discussion. Other than reference checking, avoid the need to ‘optimize’ the workshop by typing directly into the computer. Instead…

### Condense workflow in business rules

Requirements clarification in workshops often starts with abstract concepts, and then when examples are put forth, it moves into workflow discussions—”When using the system I’d do step one, then step two, and then expect X.”

These workflow examples may end up being similar with only a slight variation in one or two steps. The workflow tests contain hidden business rules, which can be extracted and put into a data-driven test. This centers the discussion on domain clarification and reduces complexity by removing irrelevant details.

### Test the walls

The rightful home of tests is on the wall—well, with a whiteboard between the tests and the wall. Big whiteboard spaces promote collaboration—the purpose of the workshop. The whiteboard sketches are captured with photos. After the workshop, the tests may be distilled and written in a tool.

<figure>
  <img src="/img/test_automation/atdd_wall1.jpg" alt="atdd_wall1.jpg">
</figure>

<figure>
  <img src="/img/test_automation/atdd_wall2.jpg" alt="atdd_wall2.jpg">
</figure>

### Use table format

Expressing business rules in tables makes them more comprehensible and assists in finding missing cases. Tables inspire clear thinking. Influential computer scientist [David Parnas is a long-time promoter](http://link.springer.com/chapter/10.1007/978-3-7091-6510-2_12#page-1) of tables for documenting requirements.

> [When documenting requirements,] writing, understanding, and discovery go on at the same time… Tabular notations are of great help in situations like this one. One first determines the structure of the table, making sure that the headers cover all the possible cases, then turns one’s attention to completing the individual entries in the table.

### Use Workflow tests

Extracting business rules and using data-driven tests is not always possible or desirable. Some requirements are just better expressed in a workflow (multi-step scenario) example. Also, data-driven business-rule tests can often be complemented with workflow examples that, in a way, link them.

Caution: When most of your tests are workflow tests, then you probably missed some business rules.

### Typical workshop agenda

How is an A-TDD requirements workshop structured? We frequently use the following agenda:

1. *Introduction*—the Product Owner welcomes everybody to the workshop and explains its purpose.
2. *Selection*—the team and Product Owner pick the items from the Product Backlog that will be worked on.
3. *Overview*—the Product Owner or representative gives a short overview of the selected requirements.
4. *Diverge*—the team splits into two or three subgroups that each pick an item and start writing examples on whiteboards. The Product Owner and representatives rotate between subgroups.
5. *Merge*—the subgroups combine and one at a time share their work with the whole group.
6. *Repeat*—the diverge-merge cycles are usually 30–45 minutes long. One workshop contains multiple cycles.
7. *Conclude*—the Product Owner summarizes the work. Then, there is a brief reflection on the workshop.
8. *Distill*—participants take photos of all the work and put them on the wiki. They might already distill some tests and document them in their A-TDD tool.

## Develop in Concurrence

After the requirements are clear, they need to be implemented. The different activities required for implementation are done in concurrence. The team extends the tests while at the same time implementing the code, writing the documentation, updating the design description, and so forth.

### Distill the tests

Many examples are created during the requirements workshop. Not all of these become tests—only the essential parts of the requirements are distilled into tests. The nonessential or duplicate parts are discarded—they have served their purpose for learning during the workshop.

How to distill tests from examples? Some techniques:

* **Duplication**—Remove duplication among examples by writing the tests in a different form. For example, a set of workflow tests might be combined into a business-rule test. Most of this should have happened during the workshop.
* **Equivalence class**—Some examples are part of the same equivalence class and therefore it is enough to keep one test. People with a testing speciality are especially valuable since equivalence-class partitioning is a classic testing technique.
* **Acceptance**—Since not all examples are of equal importance, ask the Product Owner, “What set of examples do you want to see running at the end of the iteration?”

### Use A-TDD coaches and facilitators

A-TDD is easy to do, and hard to adopt. It requires challenging deeply rooted assumptions and changes in habit. An (external) coach with experience in A-TDD and organizational change is frequently needed for this. Find a coach.

It is important to realize that the skills of a good A-TDD coach are different from those of a good TDD coach. TDD coaching is more technical, and focused on individual developers, whereas A-TDD involves the whole team. In additional to technical skills, a good A-TDD coach has excellent workshop-facilitation skills.

### Use an A-TDD Tool

* Fit is perhaps the first A-TDD tool. It was developed by Ward Cunningham in 2002. Fit tests consist of HTML tables that are executed by a piece of glue code—called a fixture. Micah and Bob Martin created an extension of Fit called FitNesse in which the tables are written in a wiki. Fitnesse also includes Slim—a slimmer execution model that offers better portability and the flexibility to explore new test syntaxes. More information can be found in the recommended readings at the end of this chapter.
* Robot Framework originates from Nokia Siemens Networks and was developed by Pekka Klärck. It was open-sourced in 2008. Robot has some similarities to Fit, such as tabular structured tests and glue code between the tables and the system. However, it also has unique features such as layering tables (user keywords).
* Cucumber was developed by Aslak Hellesøy and inspired by Dan North. It follows the given/when/then format for describing the examples. Cucumber tests are readable sentences in plain text.

### Don't use conventional test tools for A-TDD

Some product groups we worked with try to use their conventional test tools such as Lisp-based scripts or TTCN for A-TDD. This invariably fails. Why? A-TDD-style tests are created so that the Product Owner or user can read and understand the tests. But the test format—scripts—of these conventional tools are created for testers and are thus unsuitable for documenting requirements. It is nearly impossible to involve the Product Owner in writing examples using such tools.

### But do wrap conventional test tools under an A-TDD tool

Should you throw away all conventional test tools when adopting A-TDD? Perhaps not.

A graphics product group we worked with had spent years building a scripting language for automating their tests. It would take an additional few years to develop the glue code (test libraries or fixtures) between the A-TDD framework and their system under test—most of it is the same work they did with their scripting language.

An alternative is to let the glue code wrap their test scripting language and reuse their earlier work. Conventional test tools are not necessarily bad tools, but they just provide the wrong format—the wrong language—for executable specifications.

## Deliver for acceptance

The code is implemented and all the tests pass. What’s next? The A-TDD cycle, like Scrum, contains an inspect–adapt cycle where the results are delivered to stakeholders, who inspect the outcome using the tests and decide how to proceed—which requirements to implement next.

### Show tests in Sprint Review

In a Sprint Review, the team demonstrates visible progress to the Product Owner by showing the output of the iteration.

We worked with some groups that defined the demo steps during the Sprint planning. The team would spend an inordinate amount of time in demo preparation. A complete waste.

During Sprint Planning, an alternative is to define the examples that need to pass and show the progress by using these tests in the Sprint Review.

## Recommended Readings

* [*Specification by Example*](http://www.amazon.com/Specification-Example-Successful-Deliver-Software/dp/1617290084), by Gojko Adzic. This book covers several case studies about "Specification by Example". Gojko coined the term to replace all previous terms such as A-TDD.
* [*Bridging the Communication Gap*](http://www.amazon.com/Bridging-Communication-Gap-Specification-Acceptance/dp/0955683610/ref=sr_1_1?ie=UTF8&qid=1415541943&sr=8-1&keywords=bridging+communication+gap) , by Gojko Adzic. The book before Specification by Example which has a strong focus on requirements clarifications and workshops.
* [*Acceptance Test Driven Development: An Overview*](http://testobsessed.com/2008/12/acceptance-test-driven-development-atdd-an-overview/) , by Elisabeth Hendrickson. A blog post and related paper providing an overview of A-TDD by giving a detailed example of using Robot Framework.
* [*Fit for Developing Software*](http://www.amazon.com/Fit-Developing-Software-Framework-Integrated/dp/0321269349) , by Rick Mugridge and Ward Cunningham. This book has a strong focus on improving the communication of requirements by means of Fit tables.
* [*Robot Framework User Guide*](https://code.google.com/p/robotframework/wiki/UserGuide) . Does not cover A-TDD, but does provide an excellent introduction to the Robot Framework tool.
* [*Test-Driven .NET Development with FitNesse*](http://www.amazon.com/Test-Driven-NET-Development-FitNesse/dp/0955683602) , by Gojko Adzic. This book has less emphasis on A-TDD and more on FitNesse. But it does a good job in describing the tool.
