# Notas Girhus

## Docker
**Mostrar imágenes**
``docker images``

**Mostrar contenedores y sus puertos**
``docker container ls --all``

## Container
**Averiguar la IP de un contenedor**`

``docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' nombre-contenedor``

## Apache
**Reiniciar apache**
``docker exec 7.3.x-webserver service apache2 reload``

## mySQL
```sql
SET GLOBAL sql_mode='STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION';
```

## Referencia
* https://medium.com/code-kings/docker-building-a-lamp-stack-9503c62d9214
* https://hub.docker.com/r/mysql/mysql-server/