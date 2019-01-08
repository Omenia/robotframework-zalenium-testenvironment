# Boilerplate for Robot Framework testing with Zalenium

## Prerequisites

* docker
* docker-compose

## Running tests

```
docker-compose up robot
```

### Rebuild containers and run tests

```
docker-compose up --build robot
```

### Passing arguments to robot

```
ROBOT_ARGS="-v BROWSER:firefox -v SELENIUM_SPEED:2" docker-compose up robot
```

## Stop environment

```
docker-compose down
```
## Usefull URLs

View tests running in real time: http://localhost:4444/grid/admin/live
Dashboard for saved videos: http://localhost:4444/dashboard/
The Grid console http://localhost:4444/grid/console


### Pass more configuration parameters for zalenium

Zalenium is started with default parameters that include video recording. More parameters can be added to the start-command in docker-compose. See https://opensource.zalando.com/zalenium/#docker for list of available parameters. 
