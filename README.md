# THIS IS VISMA NBA-TEAMS TASK UTILIZING THEAPIGUY'S FREE-NBA API :)

## How to begin?

### FIrst check that your platform has these requirements:
* Ubuntu or other linux based OS installed
* Docker 20+  

### First, let's install dependencies for docker

//THE FILES UPLOADED HERE HAS THESE INSTALLED ALREADY BUT YOU CAN STILL USE THIS COMMAND IF YOU MAY LIKE

```bash
docker-compose run --rm composer install 
```

### How to run tests?
```bash
docker-compose run --rm phpunit
```

### How to run the program?

Help command with program documentation
```bash
docker-compose run --rm cli
```

### List all NBA teams
```bash
docker-compose run --rm cli teams
```

### List NBA teams by keyword
```bash
docker-compose run --rm cli teams boston

### List NBA games by date (date format YYYY-MM-DD)
//IF THERE ARE NONE - YOU WILL GET NO RESULTS

docker-compose run --rm cli games 2021-05-16


### You can also list games by specifying filter that you may like (let's choose: 2021-05-16)

sudo docker-compose run --rm cli games --filter date 2021-05-16

### Or you can list those games by choosing the season as you may like (let's choose: 2022)

sudo docker-compose run --rm cli games --filter season 2022
```
