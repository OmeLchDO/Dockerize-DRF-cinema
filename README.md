# Cinema API

API services for cinema management written on DRF

## Installing using GitHub and create database

- git clone https://github.com/OmeLchDO/Dockerize-DRF-cinema.git
- cd Dockerize-DRF-cinema
- python -m venv venv
- venv/Scripts/activate (for Windows)
  or source venv/bin/activate (for MacOS, Linux)
- pip install -r requirements.txt
- python manage.py migrate
- python manage.py runserver


## Install PostgresSQL and create db

create .env by example:

```
POSTGRES_HOST=<your db hostname>
POSTGRES_DB=<your db name>
POSTGRES_USER=<your db username>
POSTGRES_PASSWORD=<your db password>
```

## Run with docker

https://hub.docker.com/r/omelchdo/dockercinema

Docker should be installed

```
docker-compose build
docker-compose up
```


## Getting access

- create user via /api/user/register/
- get access token via /api/user/token/


## Features

- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie session
- Filtering movies and movie session