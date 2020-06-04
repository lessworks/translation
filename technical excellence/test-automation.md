---
title: Test Automation
order: 60
---

## Manual Tests

Agile developers emphasize the importance of automated tests. With short cycles, manual regression testing is nearly impossible. Does that mean there is no manual testing at all? No. Some manual testing is still recommended, though such testing differs from the traditional script-based manual testing.

### Automate your manual tests

Product groups often claim “It is impossible to automate tests related to a lost network connection” or “You can’t automate tests related to hardware failure” Our answer usually is “No, it is not” or “Yes, you can.”

Elisabeth Hendrickson, the author of the mini-book [*Exploratory Testing in an Agile Context*](/papers/et.pdf) , dares to state that:

> I do think that if you can write a manual script for a test, you can automate it.

It may be difficult to automate a test in *exactly the same way* as it would be carried out manually. For example, it is nearly impossible to remove the network cable automatically in a connection-lost test case. Therefore, the automated test is usually done in a different way. Instead of the cable being physically detached, the automated test instructs the driver to respond *as if* the cable were removed.

Is automating all tests worth it? According to Hendrickson:

> If it’s a test that’s important enough to script, and execute, it’s important enough to automate.

Why is this? Iterative and incremental development implies that code is not frozen at the end of the iteration but instead has the potential to be changed each iteration. Therefore, manual regression testing would mean rerunning most of the manual test--every iteration. Automating the tests therefore pays back quickly.

Especially in large-scale development with feature teams and shared code-ownership, the safety net provided by automated tests is of paramount importance. Automating tests is well worth the effort.

### Do some manual tests

Automating *all* tests might not be worthwhile or even possible. These tests may need to be done manually:

* *Tests requiring human opinion and creativity* --A person is needed to judge whether the interface looks good--usability testing. Exploratory testing by definition needs someone to decide the next step to explore.
* *Tests requiring physical movement* --For example, tests with the system in different physical configurations. These can be automated with simulation, but the real configuration might be needed for the final test run.
* *Expensive tests* --Running capacity tests on the production environment may be too expensive and is therefore done only once or twice. This delays risk. These risks should be tackled early with cheaper tests--for example, running capacity tests on a simulated environment--so that running the expensive test is merely a final check.

No false dichotomy: Try to automate all tests, but do not forget to do the manual tests when needed.

### Do exploratory testing

In [Perfect Software and Other Illusions about Testing](http://www.amazon.com/Perfect-Software-Other-Illusions-Testing/dp/0932633692), Gerald Weinberg calls it, “The Exhaustive Testing Fallacy, that it’s possible to test everything!” It is not. The number of possible scenarios to test is infinite and therefore automating all tests means infinite automation effort. Instead, automate all the anticipated tests and spend time as efficiently as possible on manual exploratory testing to find unforeseen cases.
over-view of exploratory testing

<figure>
  <img src="/img/test_automation/et.png" alt="et.png">
  <figcaption>Exploratory testing</figcaption>
</figure>

What is exploratory testing? “Simultaneous learning, test design, and test execution” [[Bach03]](http://www.satisfice.com/articles/what_is_et.shtml). This is in contrast to traditional scripted testing where test-case design and execution are separated and sequential steps—first design then execution. Exploratory testing aims at fully utilizing human creativity during test execution, using feedback and observations rather than mindlessly following a script. In exploratory testing, the tester is exploring the system, learning about it and using that information to make test-design decisions. It is best explained by an example.

Imagine that Gita is testing a 2D modeling application. First, she defines the goal of her test session—in exploratory testing this is called a mission or charter. Her charter is “Explore changing shapes by dragging the control points.” She takes a shape, drops it on the canvas, and creates a couple of control points on it. She drags one of them and observes what happens. Based on this observation (learning), she determines the next step (design) and performs it (execute). The shape takes its new form, though she notices—while dragging the control points—that the shape temporarily took a form that it probably should not have. Therefore, she continues dragging it and moving it around until she can reproduce the accidental transformation.

In the example, there is no detailed preconceived script or test case but instead an area of focus—a charter. The first step is to observe the system, and the next action is determined from that observation—this is test design. All traditional test techniques and heuristics are applied during this design step.

<figure>
  <img src="/img/test_automation/et_scripted_difference.png" alt="et.png">
  <figcaption>Exploratory testing</figcaption>
</figure>

## Automated Testing

### Create maintainable tests

“Automated tests will increase our test maintenance load” is a common objection we hear. Test maintenance will cost some effort, but a few straightforward techniques can minimize this cost:

* remove duplication in and between tests
* delete tests when not adding value
* do not test through the UI
* run tests frequently

### Remove duplication in and between tests

Code duplication causes extra complexity, obscurity, and defects—resulting in extra maintenance effort. This is as true for test code as it is for production code. Avoid this by removing the duplication.

Workflow tests are a common cause of duplication. They often consist of one mother scenario and multiple derived cases with only slight variations in them. When one step changes, all these workflow tests need to be updated. This duplication can be avoided by data-driven tests that focus on business rules or by separating the duplication into test libraries or fixtures.

We coached a team that made a common mistake—they delayed their test automation until the end of the iteration. Four days remaining and only automation tasks left. In the previous iterations, these tasks were done by the test specialist, but now they had to be done by the whole team.

They started with a one-day workshop in which the one specialist coached the other team members. After that, they split into two pairs and one triplet working in parallel on automating the tests. Something interesting happened: The team members who were experienced in programming complained about the extra effort needed because of the duplication in the tests. Previously, none of them had noticed it and the test specialist—who did not have much programming experience—never cared. Now that the whole team was involved, they cared and the quality of the tests improved immensely.

### Delete tests when not adding value

Tests serve multiple purposes. They act as requirements, as verification, and as a safety net preventing system regression.

When an existing test is not needed anymore—because it is a subset of another test—then delete it. Leaving unnecessary tests brings no benefit but still increases maintenance effort and lowers test execution speed.

### Avoid testing through the UI

User interfaces (UIs) tend to change frequently. Running your tests through the UI makes them vulnerable to these changes—even when there is no change in test logic. This increases the test maintenance effort.

Therefore, avoid testing through the UI and instead call the application logic directly through an API. Another advantage of doing this is that it speeds up your test since testing through the UI is slow.

### Run tests frequently

Long ago, we worked with a large group following waterfall develop- ment. Traditional test automation advice is to select and automate only the most important cases—with a separate automation team— after the release. So they did. At the end of the next release, they executed the tests and... they all failed. Updating them would take much time, so they decided to do all testing manually.

Executing tests once or twice a release seems efficient—fewer CPU cycles are wasted—but much will have changed and therefore many fail and cause a large batch of maintenance work. Alternatively, exe- cuting tests frequently—using a continuous integration system— uses more CPU cycles but results in less maintenance work since the effort to fix failing tests is small and straightforward. If you have a high test-maintenance load, chances are you are not executing the tests frequently enough.

### Treat non-functionals the same as functionals

Automating and continuously running non-functional tests is essential. Delaying them to the end means moving one of the biggest risks to where they hurt most. For example, if the system needs a certain performance level, test early to reach it early, and continuously run the test while new functionality is added to ensure that the system does not regress from its performance target.

Non-functionals are often treated exotically—people believe they cannot be specified and cannot be tested. This is unfortunate. In a requirements workshop, non-functionals can be considered the same as functionals, and example tests are created for clarifying them.

### Continuously run long-running tests

Non-functional tests frequently cannot be run in the normal continuous-integration-system cycle because they may take too long to execute—a stability test might take two weeks. Some product groups delay them until near the release—creating a delayed feed-back cycle. Not a good idea.

Run the long-running tests all the time in a slower continuous-integration-system cycle. Treat them as any other tests. When they fail, inform all people who checked in code. After they pass, get the latest build and immediately run them again. This way the feedback cycle is as short as it can be.

### Use virtualization or containers

In order to speed up the tests and keep the investment in hardware low, maximize the use of virtualization using [VirtualBox](https://www.virtualbox.org/) or [VMWare](http://www.vmware.com/). An alternative to virtual machines (which aren't always fast to build and easy to maintain) are linux virtual containers such as [Docker](http://www.docker.io/)

### Avoid using commercial test tools

We once coached at a company building a commercial “automated testing” tool—a GUI testing tool. The requested coaching? To learn how to do automated testing for developing their automated testing tool...

A gazillion commercial test tools are available. We rarely meet people who are actually satisfied with any of them. Most are overly complex and focus more on reporting and ‘management’ than on robust test automation. Favor free and open-source tools—made by developers solving real problems—over commercial tools.

Example of common test automation tools:

* [RobotFramework](http://www.robotframework.org/)
* [Cucumber](https://cucumber.io/)
* [Fitnesse](http://www.fitnesse.org/)
* [Selenium](http://www.seleniumhq.org/)
* [Capybara](https://github.com/jnicklas/capybara)

There are much more. The above is just a list of common tools, but new tools pop up all the time.