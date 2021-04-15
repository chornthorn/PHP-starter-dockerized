# Docker setup for PHP projects

This setup will work for your all PHP projects. You need to put these all files in your project root directory.

# This setup has included:
- PHP (7.3.x)
- MySQL (5.7.x)
- Nginx
- PHPMyAdmin
- Composer
- Custom PHP.ini & phpmyadmin.ini
### Application ports:
- Web Server: 8080
- MySQL Database: 33061
- phpMyAdmin: 8081

To start the services:

```bash
docker-compose up -d
```

To see current running containers: 
```bash
docker ps
```

To restart/stop services: 
```bash
docker-composer stop
docker-composer restart
```
SSH into a container ( You'll get container name from `docker ps` command )
```bash
docker exec -it <container name> /bin/bash
```