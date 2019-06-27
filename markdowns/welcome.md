# Behaviour Driven Development (BDD)

## What it is

>In software engineering, behavior-driven development (`BDD`) is an Agile software development process that encourages collaboration between developers, QA and non-technical or business participants in a software project.
>
>-- _Wikipedia_


> So, it's Cucumber, right ?

---

## BDD is not only Cucumber

`Cucumber` is one of Java's framework to work in `BDD`.
You may have heard of `Specflow` for .net.

In order to work, `Cucumber` and `Specflow` both rely on `Gherkin`.

---

## BDD is not only Gherkin

`BDD` comes from `Test Driven Developement` :

* Define what the tests should verify
* Ensure the test is failing
* Implement the code that will validate the test
* Ensure the test is not failing anymore

The team should thrive to define the expected behaviours of their system before developing them.

As we are talking team-wise, we need to describes a behaviour in a language that any human can understand.

### Ubiquitous language

>A ubiquitous language is a (semi-)formal language that is shared by all members of a software development team — both software developers and non-technical personnel. The language in question is both used and developed by all team members as a common means of discussing the domain of the software in question. In this way BDD becomes a vehicle for communication between all the different roles in a software project.
>
>-- _Wikipedia_

Gherkin is a ubiquitous language used by Cucumber in order to apply the Behaviour Driven Development process within a software team.

