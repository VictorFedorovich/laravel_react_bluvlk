
### Option 1

1. `git clone`
2. `create a .env file copy content from .env.example and update the values`
3. `composer install && composer update`
4. `php artisan cron:refresh-database`
5. `npm install && npm run dev`
6. `php artisan key:gen`
7. `php artisan serve`


### Option 2

## Prerequisite
Make sure you have [docker](https://docs.docker.com/install/) and [docker-compose](https://docs.docker.com/compose/install/) installed on you machine.

1. `git clone`
2. `create a .env file copy content from .env.docker and do not make any change`

run following command in terminal / power shell
```
docker-compose up -d
```

when docker will finish building the containers, access the "laravel-react-app" container using following command

`docker exec -it laravel_react_app sh`

now you will be inside container

run following commands
1. `composer install && composer update`
2. `php artisan cron:refresh-database`
3. `php artisan key:gen`
4. `npm install && npm run dev`

open browser and check the following address

`http://localhost:8100`



