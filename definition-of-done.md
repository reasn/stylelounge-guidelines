# Definition of Done

* Code reviewed
* Functional test against expected behaviour has passed
* Feature was deployed and tested on Staging environment \(if applicable, \#backend\)
* Feature was deployed to production and passed production checklist
* All subtasks are completed or all "❌" became"✅"
* Documentation updated
* Product Owner accepts the User Story

## The Basics

1. Expected behavior is fulfilled
2. All execution paths in the changed code have been run locally
3. You consider the added code to be maintainable
4. Readability &gt; performance
5. Complex structures need comments answering two questions
   * What happens here?
   * Why does it happen here?
6. You are sure that others will understand the code without your help
7. The code builds without errors
8. All tests pass
9. The test coverage of added lines of code is &gt; 70%
10. All "❌" became "✅"
11. Code doesn't violate our collected patterns \([stylelounge.gitbooks.io/patterns](https://stylelounge.gitbooks.io/patterns/)\) unnecessarily

## Code Quality

* Completed code walkthrough with 2+ developers \(or having done pair programming the thing in the first place\)

> ### Everybody
>
> Two people properly reviewed the PR
>
> ### Juniors
>
> * Two people \(at least one senior\) reviewed the PR
> * You did a walkthrough with one team member

## Reactive Microservice

* All input is validated using JSON schemas
* A list of depending subservices and necessary changes has been created
* The code has been executed using production input messages.
* Consume from a queue following the pattern: developerName-test-subserviceName-expirationDate
* Publish onto a local broker if necessary

## Requirements for Bugs

* Root cause and possible solution are documented in the issue

