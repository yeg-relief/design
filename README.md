## THIS IS NO LONGER ACCURATE DOCUMENTATION
For up to date docs, see [here](https://github.com/yeg-relief/youcanbenefit/wiki).

# YouCanBenefit
![home_page](https://github.com/yeg-relief/design/blob/master/pictures/youcan-benefit.PNG?raw=true)
[try it live](http://www.youcanbenefit.ca/)

# Documentation

If you're looking for documentation, then be sure to read the [wiki](https://github.com/yeg-relief/design/wiki).

# Purpose

`YouCanBenefit` is a web application that increases social benefit program discoverability for people of lesser means and their allies. There are similiar projects, but where I think `YouCanBenefit` differs in at least some cases, is that it takes what the user likely knows -- their demographic information -- and compares against what the user likely has trouble finding -- the available social programs. It does not save user data.

### Deployment quick-start
Want to run the app? Setup is documented [here](https://github.com/yeg-relief/design/wiki/Deployment-quick-start). 
Maybe read some other parts of the [wiki](https://github.com/yeg-relief/design/wiki) too.

# Technologies

* [Angular](https://angular.io/)
* [Caddyserver](https://caddyserver.com/)
* [Docker](https://www.docker.com/)
* [Node](https://nodejs.org/en/)
* [Typescript](http://www.typescriptlang.org/)

# Components

[screenerClient](https://github.com/yeg-relief/screenerClient) is the `web client` it is written in [Angular](https://angular.io/)/ One useful feature is the `/admin` module. It allows for an admin to configure [elasticsearch](https://www.elastic.co/products/elasticsearch) from a `gui`.

![master-screener edit](https://github.com/yeg-relief/design/blob/master/pictures/master-screener-edit.PNG?raw=true)

[api-server](https://github.com/yeg-relief/api-server) is the `api` that handles backend business logic and acts as an interface with `elasticsearch`.

[utils](https://github.com/yeg-relief/utils) are various utilities that can manage `elasticsearch` data. Used to `seed` -- create the database and put a test value in it -- `download` data or `stream` data from one `elasticsearch` instance to another.

***

[developer quickstart](https://github.com/yeg-relief/design/wiki/Developer-quick-start) hopefully a relatively simple set of instructions to start.

# Where to go next?

* read the [wiki](https://github.com/yeg-relief/design/wiki)
* look at the issues: 
    * [api-server](https://github.com/yeg-relief/api-server/issues)
    * [screenerClient](https://github.com/yeg-relief/screenerClient/issues)
    * [issue-tracker](https://github.com/yeg-relief/issue-tracker/issues)

# refactor

1. Refactor code into modules -- don't mess with implementation details just make modular.
2. Break modules apart -- turn them into seperate npm modules.
3. Test modules -- set expected code behavior
4. refactor modules -- improve code quality
5. document modules -- a diagram and a sentence or two
6. combine modules -- combine modules into application
7. Publish the code as npm modules.

# client side specific

1. split the user and admin application into two different applications
2. make the user application vanilla
3. implement progressive web application features
4. make the admin application a heavier `Angular` application. 

# server side specific

1. ~~Production~~, development and test docker builds.









