# Feature testing with Behat

## Story

Your task will be to write feature tests for `Wikipedia` search using `Behat`.

## What are you going to learn?

- write feature tests using `Behat`
- the application(s) of `Behavior-Driven Development`

## Tasks

1. Install `Behat`, `Mink Extension` and `Mink Goutte Driver` at once, using `Composer`
    - A folder named `behat` exists in the `vendor/behat` directory
    - A folder named `mink-extension` exists in the `vendor/behat` directory
    - A folder named `mink-goutte-driver` exists in the `vendor/behat` directory

2. Create a configuration file for `Behat` and `Mink Goutte Driver`.
    - The `behat.yml` file exists in the root folder
    - The file contains `context` configurations for default test suites
    - The file contains `goutte` configurations for `Wikipedia` search tests

3. Create a feature test suite for `Wikipedia` search, using `BDD` and `TDD` related search phrases, like `ATDD`, `DDD`, or `OOAD`.
    - The test suite has a `Feature` description
    - The test suite has a `Wikipedia` search `Scenario`
    - The `Scenario` has the following search phrase `Examples`:
  - BDD
  - TDD
  - ATDD
  - DDD
  - OOAD

## General requirements

None

## Hints

- Some `Behat` packages require to be installed inside a `Git repository` folder with at least 1 commit.
- You can add custom `tags` to your scenarios using the `@` sign to categorize them
  ```gherkin
  @test @bdd
  Scenario: Search for BDD
    Given I am on "/"
    When I fill in "searchInput" with "BDD"
    And I press "go"
    Then I should see "Behavior-driven development"

  @test @tdd
  Scenario: Search for TDD
    Given I am on "/"
    When I fill in "searchInput" with "TDD"
    And I press "go"
    Then I should see "Test-driven development"

  @sdlc
  Scenario: Search for SDLC
    Given I am on "/"
    When I fill in "searchInput" with "Software development life cycle"
    And I press "go"
    Then I should see "Software development process"
  ```

  Use these tags to run only the specific type of tests
  ```shell
  ./vendor/bin/behat --tags test
  ```

## Background materials

- <i class="far fa-candy-cane"></i> [A step-by-step solution guide](project/curriculum/materials/pages/guides/feature-testing-with-behat--php.md)
- <i class="far fa-book-open"></i> [What is a User Story?](https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story/)
- <i class="far fa-video"></i> [What is BDD?](https://youtu.be/3_sIQEkkoko)
- <i class="far fa-book-open"></i> [Behat - PhpStorm](https://www.jetbrains.com/help/phpstorm/using-behat-framework.html)
- <i class="far fa-video"></i> [Behaviour Driven Development and Behat](https://youtu.be/bCLlBgYQoIk)
- <i class="far fa-candy-cane"></i> [The 5 Whys Method](https://youtu.be/B-M3YlA2KDg)
