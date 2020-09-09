---
title: Отслеживание Прогресса в Спринте
order: 700
---

The Team in Scrum is self-managing, and in order to do this successfully, it must know how it is doing.  Every day, the Team members update their estimate of the effort remaining to complete their current work in the **Sprint Backlog** (Figure 6). It is also common for  someone to add up the effort remaining for the Team as a whole, and plot it on the **Sprint Burndown Chart** (Figure 7 and Figure 8). This graph shows, each day, a new estimate of how much work remains until the Team is finished. Ideally, this is a *downward* sloping graph that is on a trajectory to reach “zero effort remaining” by the last day of the Sprint. Hence it is called a *burndown* chart. And while sometimes it looks good, often it does not; this is the reality of product development. The important thing is that it shows the Team their *progress* towards their goal, not in terms of how much time was spent in the past (an irrelevant fact in terms of progress), but in terms of how much work *remains in the future* – what separates the Team from their goal. If the burndown line is not tracking downwards towards completion near the end of the Sprint, then the Team needs to adjust, such as to reduce the scope of the work or to find a way to work more effectively while still maintaining a sustainable pace.

While the Sprint Burndown chart can be created and displayed using a spreadsheet, many Teams find it is more effective to show it on paper on a wall in their workspace, with updates in pen; this “low-tech/high-touch” solution is fast, simple, and often more visible than a computer chart.

<table class="grid_table_with_header">
  <thead>
    <tr>
      <th style="text-align: center">Product Backlog Item</th>
      <th style="text-align: center">Task</th>
      <th style="text-align: center">Volunteer</th>
      <th style="text-align: center">Initial Estimate of Effort</th>
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
      <td>As a buyer, I want to place a book in a shopping cart</td>
      <td>modify database</td>
      <td>Sanjay</td>
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
      <td>create webpage (UI)</td>
      <td>Jing</td>
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
      <td>create webpage (javascript logic)</td>
      <td>Tracy and Sam</td>
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
      <td>write automated acceptance tests</td>
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
      <td>update buyer help webpage</td>
      <td>Sanjay and Jing</td>
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
      <td>Improve transaction processing performance</td>
      <td>merge DCP code and complete layer-level tests</td>
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
      <td>complete machine order for pRank</td>
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
      <td>change DCP and reader to use pRank http API</td>
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

**Figure 6.** Daily Updates of Work Remaining on the Sprint Backlog
{: .table-figure-caption}


<div>
  {% figure "img/scrum/sprint-burndown", "Figure 7. Sprint Burndown Chart", class:"two-third-sized-figure", caption: true %}
</div>

<div>
  {% figure "img/scrum/hand-drawn-sprint-burndown", "Figure 8. Visual Management: Hand-drawn Sprint Burndown Chart", class:"two-third-sized-figure", caption: true %}
</div>

Перевод статьи осуществлён [Кротовым Артёмом](https://www.facebook.com/artem.v.krotov) и [Романом Лапаевым](https://www.linkedin.com/in/romanlapaev).