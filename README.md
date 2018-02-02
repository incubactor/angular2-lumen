# Angular2-Lumen
This is example of Angular2, Laravel/Lumen, Authentication with JWT.

## Install Server

### Requirements

  - Lumen
  - Composer
  - MySQL server (should import db from ./api/dbimport.sql)
    For example:
    ```
    mysql -u dbuser -p
    mysql> CREATE DATABASE angularskeleton;
    Query OK, 1 row affected (0.00 sec)

    mysql> GRANT ALL ON angularskeleton.* TO 'dbuser'@'localhost';
    Query OK, 0 rows affected (0.02 sec)

    mysql> ^d

    /angular2-lumen/api$ mysql -u dbuser -p angularskeleton < dbimport.sql
  - Set the config values in  ./api/.env

### Install

    $ cd api
    $ composer install

### Setup & Run

Update contens in .env 

    $ php -S localhost:8000 -t public

It will run Laravel/Lumen API server on localhost:8000

## Install Client & Run

    $ cd ng2
    $ npm install
    $ npm start

It will run Angular2 lite-server on localhost:3000.

It also requires API server on localhost:8000, you can change API url in _services/api.services.ts

