# Simple APM(Apache + PHP + MariaDB)

> This project provides a smple APM(Apache + PHP + MariaDB) stack using Docker Compose. It includes a web server, a database, and phpMyAdmin for easy database management.

## Information

### Docker
|Image|Tag|Port Forwarding|Environment|
|:---:|:-:|:--:|:----|
|php|8.3-apache|8080:80| |
|mariadb|lts| - | <ul><li>`MARIADB_DATABASE` db</li><li>`MARIADB_ROOT_PASSWORD` !root1234</li></ul> |
|phpmyadmin|latest|8888:80| |

## How to run?

### 1. docker-compose up
```bash
$ docker-compose up
```

## Tips
- If you want to view the logs directly in the terminal while running docker-compose up, comment out the log volume mount in the docker-compose.yml file as shown below

    ```yml
    # - ./web/logs:/var/log/apache2
    ```