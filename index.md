---
---

This is the home of the MES code repository, where we host all the awesome tools for the Mind's Eye Society.

Confused about what all this is for? Check out our [homepage](https://www.mindseyesociety.org) for more information about our organization as a whole!

## Overview
The goal of our system is to have many lightweight language-agnostic services. The desire is to get people interested in writing in what they feel the most comfortable with, as we're a volunteer organization.

Technically, we're using a set of microservices hosted in Docker containers. Most services are REST APIs, with a single frontend service handling the UX stack. A public facing nginx server handles traffic from the outside world.

## Repositories
We have several public repos. A quick overview:

* [User Hub](https://mindseyesociety.github.io/mes-hub) - User authentication, org management, and office permissions.
* [Ballot Box](https://github.com/MindsEyeSociety/mes-ballot-box) - Member voting system.
* [MES WordPress](https://github.com/MindsEyeSociety/MES-WordPress) - WordPress theme that powers our main site.
* [Audit](https://mindseyesociety.github.io/audit) - Auditing system.

### Future Projects
We have a few future projects lined up. If you're interested in working on one of these, see below.

* Prestige
* Investigation
* Characters
* Applications
* Renewals

## Contributing
We welcome contributions! If you're a MES member, please let us know your name and MES # in PRs or issues if you wish to claim prestige.

If you want to claim a project, please contact the [NTA](mailto:nta@mindseyesociety.org), and we can get you sorted. Project leaders are expected to adhere to the rules below, be able to provided regular(ish) updates, and respond to issues and PRs in a timely fashion.

### Technologies
We use Docker, and prefer usage of Node.js, PHP, or Python for services. We can accommodate other languages however, as long as they're widely used and can be supported.

For databases, expect to use MySQL or Postgres. MongoDB or similar systems are not supported right now.

### Code Standards
All code needs to follow a code standard, ideally the [WordPress Standards](https://make.wordpress.org/core/handbook/best-practices/coding-standards/). Other standards can be used just fine, as long as it's documented somewhere, plays well with Github, and is part of the CI testing.

### Unit Tests
In order for a service to be considered complete, all endpoints require unit testing of some sort. We use [Travis](https://travis-ci.org/) to run unit tests on all PRs. UX does not have this requirement, but it'd be nice!

### Documentation
All service endpoints should be documented in Markdown, in a `/docs` folder in the repo. If your API has [Swagger](http://swagger.io/) implementation, that is also fine.
