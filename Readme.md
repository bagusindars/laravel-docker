## How to Install and Run the Project

1. ``` git clone git@github.com:bagusindars/laravel-docker.git ```
2. ``` docker-compose exec app composer install ```
3. Copy ```.env.example``` to ```.env```
4. ```docker-compose build```
5. ```docker compose up -d```
6. You can see the project on ```127.0.0.1:8081```

## How to use PostgreSQL as a database

1. Uncomment the PostgreSQL configuration inside the ```docker-compose.yml``` including: ```db``` and ```pgamdin```
2. Copy ```.env.example``` to ```.env```
3. Change ```DB_CONNECTION``` to ```pgsql```
## the DB_HOST is your service postgress or other databse service name inside docker-compose
4. Change ```DB_HOST``` to ```db``` 
5. Change ```DB_PORT``` to ```5432```
6. Open the ```pgAdmin``` on ```127.0.0.1:5050```

## How to run Laravel Commands with Docker Compose

1. ```cd src```
2. ```docker-compose exec app php artisan {your command}``` 