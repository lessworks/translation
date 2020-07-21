---
title: Acceptance Testing
order: 65
---

## Don't confusing acceptance and user-acceptance test

In the ideal situation, acceptance test and user-acceptance test are the same, but... Agile development literature uses the term “acceptance tests,” where we use the term “customer-facing tests.” However, in traditional development, “acceptance test” often means “user-acceptance test,” which might be different. Avoid misunderstandings.

<figure>
  <img src="/img/test_automation/acceptance_vs_uat.png" alt="acceptance_vs_uat.png">
  <figcaption>UAT is a subset of acceptance tests</figcaption>
</figure>

The above figure expresses the relationship in a diagram. User-acceptance test (UAT) is a part of acceptance testing in agile development. But acceptance test might also include non-UAT tests such as traditional functional or system test created by the team.

Ideally, all the acceptance testing—including UAT—is done within the iteration. However, getting the UAT in the iteration may be difficult because it requires active end-user involvement and not all customers are ready for that. In that case, UAT is excluded from the Definition of Done until the product group improves their relationship with the customer so that they can expand their Definition of Done.

## Show tests in Sprint Review

In a [Sprint Review](../framework/sprint-review.html), the team demonstrates visible progress to the Product Owner by showing the output of the iteration.

We worked with some groups that defined the demo steps during the Sprint planning. The team would spend an inordinate amount of time in demo preparation. A complete waste.

During [Sprint Planning](../framework/sprint-planning-one.html), an alternative is to define the examples that need to pass and show the progress by using these tests in the Sprint Review.

## Use acceptance test-driven development

[Acceptance test-driven development (A-TDD) or Specification by Example](specification-by-example.html) is a collaborative requirements discovery approach where examples and automatable tests are used for specifying requirements—creating executable specifications. These are created with the team, Product Owner, and other stakeholders in requirements workshops.