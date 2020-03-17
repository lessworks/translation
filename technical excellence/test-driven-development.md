---
title: Test-Driven Development
order: 50
---

## What Is Test-Driven Development

Test-driven development is a development style that drives the design by tests developed in short cycles of:

1. Write one test.
2. Implement just enough code to make it pass.
3. Refactor the code so it is clean.

<img src="/img/technical-excellence/tdd.png" width="30%">

In a language such as Java, this cycle is as short as five minutes. In older languages, with slower compilation and less automated refactoring support, this cycle is longer—perhaps twenty minutes.

Is test-driven development different in large product development? No. It is an individual developer practice and the number of people in the development does not matter.
The amount of legacy code, old technology, and embedded develop- ment does have an impact on unit testing and test-driven development. Therefore, most experiments in this section are related to these.

### A TDD cycle Should Be ...

<dl>
<dt>Short</dt>
<dd>The turnaround time for passing each test is short. It could take 5 mins per cycle.</dd>

<dt>Rhythmic</dt>
<dd>You’ll feel the rhythm distinctly - “red, green, refactor... red, green refactor...”</dd>

<dt>Incremental</dt>
<dd>You’ll know that as you write and pass more tests, working functionalities are being build up incrementally.</dd>

<dt>Design-focused</dt>
<dd>With good knowledge of software design principles, you’ll discover TDD is not a testing technique but a method of designing software.</dd>

<dt>Disciplined</dt>
<dd>TDD is a different way of developing software. To break the old habit of "code and fix" and to adopt a new habit will require discipline and persistence.</dd>
</dl>

## Why TDD?


## Coaching TDD

### Use TDD Coaches

When a client of ours reviewed a draft of the companion book, he mentioned that we ought to stress coaching more. “One of our mistakes is that we didn’t provide enough coaching,” he said. Though we agreed with him, we pointed out that since we are both consultants and provide such coaching, this advice would not be very credible. We might as well add an experiment “Try...Hire us.” Thus, we minimized the advice related to hiring coaches.

But related to test-driven development, we cannot stress strongly enough: Hire coaches! Adopting TDD means unlearning traditional programming and relearning how to design and code. We rarely meet people who were able to adopt this by self-education. Most developers need a coach to pair-program with them for days or weeks. The coach constantly reminds them to write the tests first and to really clean up the code—including the test code. He helps them apply TDD and refactoring to their real code.

Test-driven development might be the hardest agile practice to adopt, but it is also one of the biggest opportunities for improving the quality of the design and code. Hire coaches!

### Internal and external coaches

External coaches are needed when adopting TDD because the com- petence does not yet exist inside the company. But, over time, growing internal coaches reduces the dependence on externals and the cost of coaching.

That said, we have seen several attempts fail to develop internal coaches. Some reasons:

* No structure was in place to decide when and with which teams to work.
* No time was reserved for coaching. Instead the internal coaches were asked to do normal development.
* Developers were less eager to learn from internal coaches...you are never a prophet in your own land.
* Coaching skills were not appreciated and further developed. The result is that skilled internal coaches often leave to be an external coach.

Choose both internal and external coaching. Depending on either of them alone is risky but combining them can lead to good results.

## Test-driven development for a better architecture

TDD can help improve the architecture of a system. How?

When we are coaching, a frequent request is help for dealing with our client’s “inflexible architecture.” This most often boils down to problems in high coupling between components—a common problem in legacy code written without TDD because the original developer did not try to test the component in isolation.

On the other hand, when a developer creates a new component (such as a class) with TDD, or refactors a legacy component to be unit-testable, they must break the dependencies of that component so that it is testable in isolation. That requires designing (or refactoring) for dependency injection and increased use of mechanisms for flexibility: interfaces, polymorphism, design patterns, dependency injection frameworks, function pointers, and more.

In this way, TDD encourages lower coupling and simple, flexible configuration—qualities of a good architecture.