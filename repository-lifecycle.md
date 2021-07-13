# Repository Lifecycle

## When you need a new repository

* Choose a name
  * If it's a temporary repository prefix it with your name
  * Otherwise make sure that the name has been discussed with the team
* Create it on GitHub
* Go to the "Settings" tab
  * Deselect the features we don't need: Wikis, Issues, Projects
* Go to the "Collaborators & Teams" tab
* * Add the `Developers` team with `Admin` privileges
  * Add the `Product`team with `Read` privileges

## Renaming a repository

* Update documentation
  * Search our GitHub organization for mentions and update them
  * Search the drive for mentions and update them
  * Search the wiki for mentions and update them
* Use `kubectl`to check of any deployment artifacts \(e.g. deployments, config maps, ingresses, services, ...\) that may be left using the old name

## If a repository is no longer needed

* Update documentation
  * Search our GitHub organization for mentions and update them
  * Search the wiki for mentions and update them
  * Search the drive for mentions and update them
* Use `kubectl` to check of any deployment artifacts \(e.g. deployments, config maps, ingresses, services, ...\) that may be left
* Make sure there's no disks left for the service
* Make sure there's no cloud storage buckets left for the service
* Prefix its name with `trash-`
* Hide it from search results on GitHub
  * Add the `trash-access` team under "Settings" with `Admin`privileges
  * Remove the `Product` team
  * Remove the `Developers` team \(⚠️ this must be the last step because you'll loose access\)

