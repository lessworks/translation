---
title: Sprint Planning
order: 500
---

**Summary**: A meeting to prepare for the Sprint, typically divided into two parts (part one is “what” and part two is “how”).
**Participants**: Part One: Product Owner, Team, Scrum Master. Part Two: Team, Scrum Master, Product Owner (optional but should be reachable for questions)
**Duration**: Each part is timeboxed to one hour per week of Sprint.

At the beginning of each Sprint, the **Sprint Planning Meeting** takes place. It is divided into two distinct sub-meetings, the first of which is called **Sprint Planning Part One**.

In **Sprint Planning Part One**, the Product Owner and Team review the high-priority items in the Product Backlog that the Product Owner is interested in implementing this Sprint. Usually, these items will have been well-analyzed in a previous Sprint (during Product Backlog Refinement), so that at this meeting there are only minor last-minute clarifying questions.  In this meeting, the Product Owner and Team discuss the goals and context for these high-priority items on the Product Backlog, providing the Team with insight into the Product Owner’s thinking. Part One focuses on understanding *what* the Product Owner wants and *why* they are needed. At the end of Part One the (always busy) Product Owner may leave although they must be available (for example, by phone) during Part Two of the meeting.

In Part One, the Team and the Product Owner may also devise the **Sprint Goal**. This is a summary statement of the Sprint objective, which ideally has a cohesive theme. The Sprint Goal also gives the Team scope-flexibility regarding what they may actually deliver, because although they may have to remove some item (since the Sprint is timeboxed), they should nevertheless commit to delivering something tangible and “done” that is in the spirit of the Sprint Goal.

How big should the items be that are taken on in a Sprint? Each item should be split small enough so that it is estimated to require considerably less than the whole Sprint. A common guideline is that an item is estimated small enough to complete within one fourth or less of a Sprint by the whole Team.

**Sprint Planning Part Two** focuses on *how* to implement the items that the Team decides to take on. The Team forecasts the amount of items they can complete by the end of the Sprint, starting at the top of the Product Backlog (in others words, starting with the items that are the highest priority for the Product Owner) and working down the list in order. **This is a key practice in Scrum: The Team decides how much work it will complete, rather than having it assigned to them by the Product Owner**. This makes for a more reliable forecast because the Team is making it based on its own analysis and planning. While the Product Owner does not have control over how much the Team signs up for, he or she knows that the items are drawn from the top of the Product Backlog – in other words, the items that he or she has rated as most important. The Team has the ability to lobby for items from further down the list; this usually happens when the Team and Product Owner realize that something of lower priority fits easily and appropriately with the high priority items.

The Sprint Planning Meeting will often last several hours, but no more than four hours for a two-week Sprint – the Team is making a serious forecast to complete the work, and this requires careful thought to be successful. Part One and Part Two are of equal timeboxed lengths; for a two-week Sprint each part is two hours maximum.

Scrum does not define how to exactly do Sprint Planning Part Two.  Some teams use their velocity from the previous Sprints to guide how much to aim for.  Other teams will use a more fine-grained approach of first calculating their capacity.

When using the capacity approach, the Team, in Sprint Planning Part Two, calculates how much time each team member has for Sprint-related work. Most teams assume that the team members can only focus on Sprint-related work for 4-6 hours per day – the rest of the time goes to email, lunch breaks, facebook, meetings, and drinking coffee . Once the capacity is determined, the Team needs to figure out how many Product Backlog items they can complete in that time, and how they will go about completing them.  This often starts with a design discussion at a whiteboard.  Once the overall design is understood, the Team decomposes the Product Backlog items into fine-grained work.  Before taking the Product Backlog items, the Team may focus on generating tasks for an improvement goal created in the previous Sprint’s Retrospective. Then, the Team selects the first item on the Product Backlog – the Product Owner’s highest priority item  – and work their way down until they are ‘full’. For each item they create a list of work which consists of either decomposed Product Backlog items into tasks or, when the Product Backlog item are so small they would only take a couple hours to implement, simply the Product Backlog item. This list of work to be done during the Sprint is called the **Sprint Backlog** (Figure 4 and Figure 5).

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
      <td></td>
      <td style="text-align: center">5</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>create webpage (UI)</td>
      <td></td>
      <td style="text-align: center">8</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>create webpage (javascript logic)</td>
      <td></td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>write automated acceptance tests</td>
      <td></td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>update buyer help webpage</td>
      <td></td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
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
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>complete machine order for pRank</td>
      <td></td>
      <td style="text-align: center">8</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td></td>
      <td>change DCP and reader to use pRank http API</td>
      <td></td>
      <td style="text-align: center">13</td>
      <td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
  </tbody>
</table>

**Figure 4.** Example of one way to create a Sprint Backlog
{: .table-figure-caption}

At the end of the Sprint Planning Meeting, the Team sets a realistic target for what they believe they can deliver by the end of the Sprint. Traditionally, this was called a Sprint Commitment – the team commits to doing the best they can to reach their target. Unfortunately, this was sometimes misinterpreted as a written-in-blood promise rather than the team seriously “going for it.” To avoid this confusion, the sprint-target is now called a ‘forecast” which is communicated to the Product Owner.

Scrum encourages multi-skilled workers, rather than only “working to job title” such as a “tester” only doing testing. In other words, Team members “go to where the work is” and help out as possible. If there are many testing tasks, then *all* Team members may help. This does not imply that everyone is a generalist; no doubt some people are especially skilled in testing (and so on) but Team members work together and learn new skills from each other. Consequently, during task generation and estimation in Sprint Planning, it is not necessary – nor appropriate – for people to volunteer for all the tasks “they can do best.” Rather, it is better to only volunteer for one task at a time, when it is time to pick up a new task, and to consider choosing tasks that will on purpose involve learning (perhaps by pair work with a specialist). This is one reason for not pre-assigning tasks during Sprint Planning, rather this should be done on an ‘as needed’ basis during the Sprint.

All that said, there are *rare* times when *John* may do a particular task because it would take far too long or be impossible for others to learn – perhaps John is the only person with any artistic skill to draw pictures. Other Team members could not draw a “stick man” if their life depended on it. In this rare case – and if it is not rare and not getting rarer as the Team learns, there is something wrong – it may be necessary to ask if the total planned drawing tasks that *must* be done by John are feasible within the short Sprint.

Many Teams have a Sprint Backlog in the form of a wall-sized task board (often called a **Scrum Board**) where tasks (written on Post-It Notes) migrate during the Sprint across columns labeled “To Do,” “Work In Progress,” and “Done.” See Figure 5.

<div>
  {% figure "img/scrum/daily-scrum", "Figure 5. Visual Management - Sprint Backlog tasks on the wall", caption: true,  class:"half-sized-figure pull-right" %}
</div>

One of the pillars of Scrum is that once the Team sets its target for the Sprint, any additions or changes must be deferred until the next Sprint. This means that if halfway through the Sprint the Product Owner decides there is a new item he or she would like the Team to work on, he cannot make the change until the start of the next Sprint. If an external circumstance appears that significantly changes priorities, and means the Team would be wasting its time if it continued working, the Product Owner or the Team can terminate the Sprint. The Team stops, and a new Sprint Planning meeting initiates a new Sprint. The disruption of doing this is usually great; this serves as a disincentive for the Product Owner or Team to resort to this dramatic decision.

There is a powerful, positive influence that comes from the Team being protected from changing goals during the Sprint. First, the Team gets to work knowing with absolute certainty that its goal will not change, that reinforces the Team’s focus on ensuring completion. Second, it disciplines the Product Owner into really thinking through the items he or she prioritizes on the Product Backlog and offers to the Team for the Sprint.

By following these Scrum rules the Product Owner gains two things. First, he or she has the confidence of knowing the Team has committed to do its best to complete a realistic and clear set of work it has chosen. Over time a Team can become quite skilled at choosing and delivering on a realistic forecast. Second, the Product Owner gets to make whatever changes he or she likes to the Product Backlog before the start of the next Sprint. At that point, additions, deletions, modifications, and re-prioritizations are all possible and acceptable. While the Product Owner is not able to make changes to the selected items under development during the current Sprint, he or she is only one Sprint’s duration or less away from making any changes they wish. Gone is the stigma around change – change of direction, change of requirements, or just plain changing your mind – and it may be for this reason that Product Owners are usually as enthusiastic about Scrum as anyone.