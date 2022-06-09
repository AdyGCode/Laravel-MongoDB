# NMT Laravel Plus Base Project

Starter Project for students at North Metropolitan TAFE

Contains:

- Laravel 9,
- MongoDB,
- MariaDB, - *we use MariaDB to replace MySQL for our work at NMT*
- Minio,
- Selenium,
- Redis,
- Memcached,
- MailHog,
- Mongo-Express.

# Installation

1) Create your own project as normal, replacing `example-app`
   with the name of your application.
    - `curl -s https://laravel.build/example-app?with=mariadb,redis,minio,mailhog,memcached,meilisearch,selenium | bash`
2) Perform `sail up` to run the base application
3) Run the command: `sail artisan vendor:publish --tag=sail-docker`
4) Perform `sail down` (or use `CTRL`+`C`) to stop the container
5) Replace the existing `docker-compose.yaml` with the one from this
   project.
6) Replace the existing `docker/8.1/Dockerfile` with the one from your
   project.
7) Perform `sail up` to re-run the application. It should now have
   mongodb and mongo-express running as part of the development
   environment.

# Additional Laravel packages

- Laravel Breeze
- Spatie ...
-

## Publish package configurations

Each publication of a package configuration is optional. It will be
dependent on your project's requirements.

```shell
sail artisan vendor:publish --tag=ignition-config 
sail artisan vendor:publish --tag=laravel-errors  
sail artisan vendor:publish --tag=laravel-mail
sail artisan vendor:publish --tag=laravel-notifications  
sail artisan vendor:publish --tag=laravel-pagination
sail artisan vendor:publish --tag=sail-docker
sail artisan vendor:publish --tag=sanctum-config 
sail artisan vendor:publish --tag=sanctum-migrations
```

Run the following commands:

```shell

  ```
