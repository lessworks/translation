---
title: Requirement Areas
order: 20
---

Feature teams scale nicely, but when their number goes above eight teams additional structure is needed. Requirement areas provide this structure and complement the concepts behind feature teams. A requirement area is a categorization of the requirements leading to different views of the Product Backlog.

The [Product Owner](../framework/product-owner.html) (PO) groups every Product Backlog item under exactly one requirement category—its requirements area. After this, he generates different views on the overall Product Backlog—called an Area Backlog. The Area Backlogs are prioritized by an Area Product Owner who specializes in part of the product—from a customer perspective. Each Requirement Area has several feature teams working from the Area Backlog, as shown in Figure 1.

<div>
  {% figure "img/less-huge/requirement-areas", "Requirement Areas" %}
</div>

Requirement areas are scaled-up feature teams. Scaling up by structuring teams according to the product’s architecture is called development areas. The table below summarizes the differences.

| Requirement Area                                 | Development Area                        |
|:------------------------------------------------:|:---------------------------------------:|
| organized around customer-centric requirements   | organized around product’s architecture |
| collective subsystem code ownership              | code ownership per subsystem            |
| temporary in nature; should change over the lifetime of the product, but not at every iteration | tends to be more fixed over the lifetime of the product |
| focus on the customer, using customer language   | focus on the architecture, using technology language |
{: .grid_table_with_header}

Development areas are *not* recommended and are only shown to show the contrast with Requirement Areas.
