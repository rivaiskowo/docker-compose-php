## Docker Compose for Web Developer
### Overview
Docker Compose setup to run multiple PHP version with Apache and MySQL
### Install
- `git clone https://github.com/rivaiskowo/docker-compose-php`
- `cd docker-compose-php`
- `docker compose up -d`
### Configuration
- The webroot is at `./htdocs/`
- php.ini for php5.6 file in `./php56/php.ini`
- php.ini for php7.2 file in `./php72/php.ini`
- php.ini for php7.3 file in `./php73/php.ini`
- php.ini for php8.1 file in `./php81/php.ini`
- php.ini for php8.2 file in `./php8w/php.ini`
- Database access
    ```
    host: db
    user: root
    password: root (password from docker-compose.yml)
    port: 3306
    ```
### Running
- http://localhost:56/info.php - php5.6
- http://localhost:72/info.php - php7.2
- http://localhost:73/info.php - php7.3
- http://localhost:81/info.php - php8.1
- http://localhost:82/info.php - php8.2
