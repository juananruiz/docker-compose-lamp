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

**Acceder al servidor por terminal**
``docker-compose exec webserver bash``

**Habilitar nuevos módulos**
Editar el fichero ``./bin/webserver/Dockerfile`` y luego reconstruir la imagen con ``docker-compose build webser```

## mySQL
Si al acceder a la intranet sale un error de SQL GROUP BY, ejecutar esta consulta:
```sql
SET GLOBAL sql_mode='STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION';
```



## Referencia
* https://github.com/sprintcube/docker-compose-lamp
* https://medium.com/code-kings/docker-building-a-lamp-stack-9503c62d9214
* https://hub.docker.com/r/mysql/mysql-server/
* https://linuxconfig.org/how-to-create-a-docker-based-lamp-stack-using-docker-compose-on-ubuntu-18-04-bionic-beaver-linux
* https://www.atareao.es/tutorial/docker/
