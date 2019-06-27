# Gherkin

## What is Gherkin

Gherkin is a language.

>Language, a system of conventional spoken, manual, or written symbols by means of which human beings, as members of a social group and participants in its culture, express themselves.
>
> -- Encyclopaedia Britannica

Gherkin uses a system of conventions in order to have business, QA and developers express and understand themselves.

## What Gherkin looks like

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
