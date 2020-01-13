# Treeherder developer experience proposal

**Mentor:** Armen Zambrano

**Email:** armenzg@mozilla.com

## Project Description

[Treeherder](https://github.com/mozilla/treeherder) is "a system for managing CI data for Mozilla projects".

## Skills Required

An applicant needs to be experienced in the following technologies:

* Git/Github
* Python
* Django
* Docker
* MySql
* Celery

An applicant needs the following skills:

* Contributing to Open Source
* Think critically
* Good reading comprehension
* Do independent research
* Enjoy working with others
* Be productive with little supervision
* Able to work remotely

## Project Details

Setting up Treeherder locally has improved in the last year by introducing Docker. If you look at the
[docker-compose.yml](https://github.com/mozilla/treeherder/blob/master/docker-compose.yml)
file you will see that it starts up Redis, MySql, RabbitMq and even the frontend app.

The set up cost has been reduced, however, the development experience needs to be improved.

All work will be planned in the following [kanban board](https://github.com/mozilla/treeherder/projects/3).

The project will focus on:

* Removing any remaining manual steps to the Docker set up (e.g. data consumers and credentials)
* Solve MySql data initialization problems
* Improve the Python development integration with VS Code
* Automatic error detection (e.g. linting issues)
