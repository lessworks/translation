---
title: Unit Testing
order: 40
---

## What Is Unit Test?

**Unit Test**s are software programs written to exercise other software programs (called **Code Under Test**, or **Production Code**) with **specific** preconditions and verify the **expected behaviour**s of the CUT. 

Unit tests are usually written in the same programming language as their code under test.

Each **unit test** should be small and test only limited piece of code functionality. Test cases are often grouped into **Test Groups** or **Test Suites**. There are many open source **unit test framework**s. The popular ones usually follow an **xUnit** pattern invented by [Kent Beck](http://c2.com/cgi/wiki?KentBeck "Kent Beck"), for example, JUnit for Java and CppUTest for C/C++.

Unit tests should also run very fast. Usually, we expect to **run hundreds of unit test cases within a few seconds**.

## Why Unit Test

The purpose of unit testing is not for finding bugs. It's a **specification** for the expected behaviours of the code under test. The code under test is the implementation for those expected behaviours. So unit test and the code under test are used to check the correctness of each other, and protect each other. Later when someone changed the code under test, and it changed the behaviour that is expected by the original author, the test will fail. If you code is covered by reasonable unit test, you can maintain the code without breaking the existing feature. That's why Michael Feathers define **legacy code** as _code without unit test_.

<img src="/img/technical-excellence/unit_test.png" width="60%">

The purpose for unit testing is rather protect what we have implemented than to find any defects, just like the anchors set by a rock climber along his way up the rock. These anchors help him to protect what he has achieved.

### Purpose of Unit Test

The purpose of unit test can be summarised as:

* Facilitates changes
  * It protects the behaviours decided by the previous programmers. So that people can change the code without breaking the existing features.
* Simplifies integration
  * Unit test tests the basic units of the program, the functions and the classes. It makes sure the basic units are functioning as expected. When these units are integrated together, we can separate the integration problems (the coupling problems) from the unit internal problems (the cohesion problems).
* Documentation
  * Well-written unit test can be used as documentation for the functionality of the code under test. Unit test contains information typically you cannot find from the code under test, for example, the design purpose of the original programming who wrote the code, and how the code is expected to be used. Unit test as documentation, unlike other traditional documentation, it doesn't "lie". Because if it lies, the test would fail. And that indicates either the test or the code is wrong.
* Design tool
  * Unit test is also an important design tool. Unit test requires testability from the code understand. Easy-to-test usually means easy-to-use. So unit test could be used to make sure the design has consideration from the perspective of use, rather than only from the perspective of implementation. Testable code needs better modularity and fewer dependencies. So that the unit test can easily take a small part of the code under test (a "unit") without taking care of the overwhelming amount of dependencies. So unit test could be used to make sure the design has "high cohesion, low coupling".

### Why on "Unit" Level?

"Yes, it's important to use automated test to protect the existing functionalities. But why does it need to be on the unit level?"

You might wonder. Why don't we just use thorough automated functional or system tests to protect the program?

**Total cost of ownership** -- Unit test is based on the abstraction level of the programming language. It's just some code exercising other code. It doesn't need to run in the same environment as the production. For compiled programming language, it doesn't even need to use the same compiler as the production. The creating and running cost of unit test is very low. If designed properly, the cost of maintaining is also very low. You may not get the same level of confidence from one successful unit test case as you can get from a functional test. You will need many small unit test cases to get approximately the same level of confidence. But the cost of these small unit test cases is still much lower than owning a few functional test cases.

If a software code base hasn't got any unit test for the past 2 years, there will be extra cost for applying unit test to this code base. The cost comes mostly from two sources:

1. The cost of applying a test framework to the code project. This is relatively easier for dynamic programming languages like Python, Ruby or Javascript. Usually, it's also trivial for Java and C# project. It can be quite tricky for C/C++ project. No matter easy or hard, this is just one-time investment.
2. The existing code base is not testable. The code was designed without considering the testability. Applying unit test to this kind of code base often involves improving the current design. Doing so doesn't only increase the cost of creating test, but also has potential cost of introducing new bugs by changing the design. So applying unit test to existing code base should be combined with other works that need the change from the code under test -- when you have to change that piece of code regardless.

**Internal Quality vs. External Quality** -- High level automated test like functional test and system test checks the external quality of the software. External quality means how well the software is functioning according to the requirement. Unit test is not as effective as the functional test in protecting the external quality. On the other hand, unit test ensures some of the internal qualities of the software. Internal quality here means the testability of the code and how well the code is protected. A testable design is in general a good design. Other levels of automated test cannot serve this purpose as well as unit test.

**Quality of feedback** When you passed a functional test, you could be very confident about the functionality you just tested. But when you found it fail, usually you need to do some debugging to see what is wrong. Unit test might be able to give you more precise information about what is working and what is broken.

Unit test is on the abstraction level of the programming language. When running unit test, everything should happen just within the CPU and memory. And each test case should be small. Therefore, it should run very fast. Typically, you should be able to run hundreds of unit tests within a few seconds. Including the compiling or other preparation time, the whole process of running unit test should take less than 1 minute.

Unit test should also be repeatable. If nothing changes, unit test runs should always return the same result.

If the unit test is very fast and repeatable, programmers can run it as often as they want, e.g. every a few minutes. The unit test will continuously provide quality feedback to the programmer. So that the programmer can go with a steady progress and focus on more important things rather than spending too much energy on trivial issues.

<img src="/img/technical-excellence/test_levels.png" width="50%">

A reasonable automated test structure should be like a pyramid. At the bottom are a lot of unit test cases. In the middle are much fewer integration level test cases. On the top, there are even fewer functional/system level tests.

## Common Misconceptions of Unit Test

### Unit test is not as important as the production code

It is true that in the end, it's production code that makes the product. But most software products have evolutionary life cycles. The code is not static. It changes over time. Code without unit test does not have the necessary protection when being changed. Unit test also contains important information that is not included in the production code.

So unit test is just as important as the production code. They should be **in the same SCM repository**. They should follow the same coding standard as the production code.

### Unit Test is done by testing engineers

The purpose of unit test is not for finding bugs. Technically, it _checks_ rather than _tests_ if the code under test has implemented the behaviour intended by the programmer who designed it. So the reasonable choice is just let the same programmer writes both the test and the code under test.

It's also encouraged to have two or more people pair up to do the programming together. They write the unit test and the code under test together. There are many fun ways of _pair-programming_. You may find more information in the Test-Driven Development section.

### You can write unit test without changing the code under test

This is often not true. If the code doesn't have good testability, you might still be able to write unit test for it technically. But the unit test written for non-testable code is usually very hard to maintain and understand. Therefore, it doesn't make much sense to have it.

**The secret of unit test is not about writing test, but writing testable code under test.** We want testable code and easy test, which is a win-win. We don't want non-testable code and hard-to-maintain code, which is a lose-lose.

### I can add unit test later

Well, try asking the rock climbers to set their anchors later.

<img src="/img/technical-excellence/unit_test.png" width="40%">

## Good Unit Test Patterns

### No news is good news

If the test passes, it should just print OK (and perhaps some dots to show the progress). No other information.

<img src="/img/technical-excellence/unit_test_success.png" width="500px">

Rule of thumb:

> No human intervention should be needed to get ready for the test, running the test cases or checking the result.

And when it fails, it should provide precise information. The goal is to limit the amount of time you spend on debugging when the test fails.
<img src="/img/technical-excellence/unit_test_fail.png" width="342px">

### Arrange, Act, Assert

A good pattern to follow in a unit test is "**AAA**": **Arrange**, **Act** and **Assert**. 

If you can easily find this pattern in each of your test cases, your tests should be easy to understand, and they should be fairly specific and to the point. One unit test case should test only one thing. Therefore, there should be only one set of AAA in one test case. A test case shouldn't be very long (longer than 10 lines of code) if it follows the AAA pattern.

<div class="inner_cell">
    <div class="input_area">
<div class="highlight"><pre><span class="kn">import</span> <span class="nn">unittest</span>
<span class="k">class</span> <span class="nc">TestGroupForTextWrapping</span><span class="p">(</span><span class="n">unittest</span><span class="o">.</span><span class="n">TestCase</span><span class="p">):</span>
    
    <span class="k">def</span> <span class="nf">test_should_have_no_wrapping_when_string_length_is_5_and_line_width_is_10</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
        <span class="c"># Arrange:  Arrange all necessary preconditions and inputs. </span>
        <span class="n">wrapper</span> <span class="o">=</span> <span class="n">TextWrapper</span><span class="p">(</span><span class="n">width</span><span class="o">=</span><span class="mi">10</span><span class="p">)</span>
        
        <span class="c"># Act:  Act on the object or method under test. </span>
        <span class="n">wrapped</span> <span class="o">=</span> <span class="n">wrapper</span><span class="o">.</span><span class="n">wrap</span><span class="p">(</span><span class="s">"a"</span> <span class="o">*</span> <span class="mi">5</span><span class="p">)</span>
        
        <span class="c"># Assert:  Assert that the expected results have occurred. </span>
        <span class="bp">self</span><span class="o">.</span><span class="n">assertEqual</span><span class="p">([</span><span class="s">"a"</span> <span class="o">*</span> <span class="mi">5</span><span class="p">],</span> <span class="n">wrapped</span><span class="p">)</span>
</pre></div>

</div>
</div>

### Behaviour Driven Development (BDD) Style

Similar to the **AAA** pattern, the **BDD** style uses three other keywords to specify each test case: **Given**, **When** and **Then**. (You can also use **And** as another keyword.)

    Given The Text Wrapper's Width Defined As 10
    And Using '-' As Word Connector
    When The Wrapper Wrap Text Length is Less Than 10
    Then The Text Should Not Be Wrapped
    
As you can see, "given-when-then" maps to "arrange-act-assert" pretty well. They both simply define a state transition of a Finite State Machine (FSM). You can find more on this in the [Uncle Bob's article](https://sites.google.com/site/unclebobconsultingllc/the-truth-about-bdd). Some differences:

* BDD is more "outside-in", which means that it emphasises more the external behaviour
* With BDD, you need to define a **domain specific language** to write your test specifications. Because of this, usually you'll need a different framework. One example for Python is [behave](http://pythonhosted.org/behave/).

### The Golden Rule Of a Unit Test

In general, a good rule for unit test case is:

> **Each unit test case should be very limited in scope.**

So that:

* When the test fails, no debugging is needed to locate the problem.
* Tests are stable because dependencies are simple.
* Less duplication, easier to maintain.

There is no secret to write good unit test. In order to write good unit test, you need to create easy-to-test design.