# How to use Gherkin

## How to NOT use Gherkin

```gherkin
Feature the login

Scenario login
    Given the login page
    Then the login page is visible
    When I enter my email
    And my password
    And I click submit
    Then I see the welcome message
    When there is a welcome message set in the database
```

`Feature` : What value am I adding ?
What am I testing here ?
