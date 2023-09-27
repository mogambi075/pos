## Server Requirements

- PHP version `7.2` to `7.4` are supported, PHP version `≤5.6` and `8.0` are NOT supported. Please note that PHP needs to have the extensions `php-gd`, `php-bcmath`, `php-intl`, `php-openssl`, `php-mbstring` , `php-curl` and `php-xml` installed and enabled.
- MySQL `5.5`, `5.6` and `5.7` are supported, also MariaDB replacement `10.x` is supported and might offer better performance.
- Apache `2.2` and `2.4` are supported. 

## Local install

2. Create/locate a new MySQL database to install Open Source Point of Sale into.
3. Execute the file `database/database.sql` to create the tables needed.
4. Unzip and upload Open Source Point of Sale files to the web-server.
5. Open `application/config/database.php` and modify credentials to connect to your database if needed.
6. Open `application/config/config.php` and swap the encryption key with your own.
7. Go to your install `public` dir via the browser.
8. Log in using
   - Username: admin
   - Password: pointofsale
9. Enjoy!

## Local install using Docker

OSPOS can be deployed using Docker on Linux, Mac, and Windows. Locally or on a host (server).
This setup dramatically reduces the number of possible issues as all setup is now done in a Dockerfile.
Docker runs natively on Mac and Linux. Windows requires WSL2 to be installed. Please refer to the Docker documentation for instructions on how to set it up on your platform.

**Be aware that this setup is not suited for production usage! Change the default passwords in the compose file before exposing the containers publicly.**

Start the containers using the following command

```
    docker-compose up
```

