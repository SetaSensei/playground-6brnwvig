# Behaviour Driven Development (BDD)

## What it is

>In software engineering, behavior-driven development (BDD) is an Agile
>software development process that encourages collaboration between
>developers, QA and non-technical or business participants in a software
>project.
>
>-- _Wikipedia_

## BDD is not only Cucumber

Cucumber is one of Java's framework to work in BDD.
You may have heard of Specflow for .net.

In order to work, Cucumber and Specflow both rely on Gherkin.

## BDD is not only Gherkin

BDD comes from Test Driven Developement :

* Define what the tests should verify
* Ensure the test is failing
* Implement the code that will validate the test
* Ensure the test is not failing anymore

Appiled to BDD, team should thrive to define the expected behaviours of their system before developing them.

As we are talking team-wise, we need to describes a behaviour in a language that any human can understand.

## Ubiquitous language

>A ubiquitous language is a (semi-)formal language that is shared by all members of a software development team — both software developers and non-technical personnel. The language in question is both used and developed by all team members as a common means of discussing the domain of the software in question. In this way BDD becomes a vehicle for communication between all the different roles in a software project.
>
>-- _Wikipedia_

Gherkin is a ubiquitous language used by Cucumber in order to apply the Behaviour Driven Development process within a software team.

## What Gherkin is

```gherkin
Feature [What is expected from my system on a business point of view]

Scenario [What will be tested next]
    Given [an initial state of my system]
    When [an event iccurs in my system]
    Then [My system should have the corresponding state]
```

Example :

```gherkin
Feature Every returned item goes back in stock

Scenario Refunded items are added back to stock
    Given a customer alerady bought a red cap
    And current stock of red cap is 10
    When a clercks register the refund for the red cap
    Then the stock of red cap is updated to 11
```
