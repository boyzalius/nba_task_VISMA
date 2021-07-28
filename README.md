# This is a task for a VISMA company utilizing theapiguy's freenba API :)

## Introduction

Hi, this is a skeleton app for your assessment. It will help you to deal your task without building the app from the scratch!

How to use it?
* Implement the business logic under `src/` directory
* Write your unit tests which should be located in here `test/`

## How to begin?

### First check that your platform has these requirements
* Ubuntu or other linux based OS
* Docker 20+
            
This program should also work even on Windows, but that was not tested yet.

### Firstly, let's install dependencies
//THOSE ARE ALREADY INSTALLED IN THIS REPO, BUT YOU CAN STILL EXECUTE THE COMMAND IF YOU MAY LIKE

```bash
docker-compose run --rm composer install
```

### How to run tests?
```bash
docker-compose run --rm phpunit
```

### How to run the program?

Execute help command with program documentation
```bash
docker-compose run --rm cli
```

List all NBA teams
```bash
docker-compose run --rm cli teams
```

List NBA teams by input keyword
```bash
docker-compose run --rm cli teams boston
```

List NBA games by input date (date format YYYY-MM-DD) let's choose 2021-05-16
```bash
docker-compose run --rm cli games 2021-05-16
```
Or by specifying filter
```bash
sudo docker-compose run --rm cli games --filter date 2021-05-16
```

Or by choosing a seasonal year

```bash
sudo docker-compose run --rm cli games --filter season 2022
```





