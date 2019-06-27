# Gherkin

## What is Gherkin

`Gherkin` is a language.

>Language, a system of conventional spoken, manual, or written symbols by means of which human beings, as members of a social group and participants in its culture, express themselves.
>
> -- Encyclopaedia Britannica

`Gherkin` uses a system of conventions in order to have business, QA, developers and any person -be it technical or not- involved in a product express and understand themselves.

> Where does Cucumber fits in ?
>
> -- _Still the same person_

`Gherkin` is a [ubiquitous language](annexes.md#ubiquitous-language) used by `Cucumber` in order to apply the Behaviour Driven Development process within a software team.

## What Gherkin looks like

```gherkin
Feature [What is expected from my system on a business point of view]

Scenario [What will be tested next]
    Given [an initial state of my system]
    When [a single event occurs in my system]
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

### Feature

Represents the value that is to be added by the developement.
It can be directly linked to the user story.

### Scenario

Gives precisions on what needs to be tested.
There is usually more than one scenario per feature.

### Given - When - Then

Following the [Triple A](annexes.md#triple-a) rule, gives the step by step actions to ensure the scenario is developed.

If `Given` or `Then` recquire more than one step, one is allowed to use `And` to add sequential following steps.

`Then` should not have `And` as each scenario should only check one single event triggering a change. Actions can be defined in the `Given` phase to set the system in the correct state.

