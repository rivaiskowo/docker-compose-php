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
- php.ini for php8.1 file in `./php81/php.ini`
- Database access
    ```
    host: db
    user: root
    password: root (password from docker-compose.yml)
    port: 3306
    ```
### Running
- http://localhost:8056/info.php - php5.6
- http://localhost:8072/info.php - php7.2
- http://localhost:8081/info.php - php8.1
### Support Me
#### Saweria
- https://saweria.co/rivaiskowo

![Saweria](https://user-images.githubusercontent.com/6821901/234471532-d14177c1-a2f5-411d-9510-e7bdf1d36d7c.png)
