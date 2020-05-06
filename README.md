# npfw
Docker for Nginx, Php-fpm and workspace (Laradock/Laradock)

Create a folder name "src" in parallel with "npfw" with index.php file in public folder as demonstrated in below figure:
```tree
.
├── npfw
└── src
    ├── public
        ├── index.php
```

index.php
```php
<?php
phpinfo();
?>
```

The repository consists of docker files for multiple containers:
``` tree
├─php-fpm
├─nginx
├─workspce 
├─php-worker
├─mysql
├─phpmydmin
├─neo4j
```

Out of all the container currently I am focusing on nginx php-fpm and workspace.

Use below command to start the containers 
```bash
docker-compose up -d nginx php-fpm workspace
```
