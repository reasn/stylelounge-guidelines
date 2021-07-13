# Refactoring

* Only continuous refactoring keeps an application alive. 
* Refactoring requires a conscious and continuous balance between two goods
  * Focus on the task at hand \(after all we want to deliver value\)
  * Improve the code base
* Refactoring takes time, usually more than estimated. Huge unplanned refactorings will prevent you from \(creating \| publishing \| deploying \| saving the day\).

## Guidelines

* Separate refactoring from feature branches. Using change sets and IDE support this is ridiculously easy!
* Have peers review refactoring PRs while working on the next ones to keep things small
* Discuss the tradeoff for individual refactorings with the team to build a shared understanding
* Sometimes it's better to create a separate follow-up ticket and add your feature to the original codebase 
* Keep the big picture in mind:
  * Are you updating the syntax of something that will never be touched or thrown again soon?
  * Does a rewrite make more sense?

