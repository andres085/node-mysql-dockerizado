# MySQL Dockerizado

### Breve descripción.
El repositorio consiste en un contenedor con dos bases de datos MySQL para desarrollo y testing.

### Obtener proyecto para comenzar.
Puede obtener el proyecto usando el comando:
```
# HTTPS
git clone https://github.com/andres085/node-mysql-dockerizado.git
# SSH
git clone git@github.com:andres085/node-mysql-dockerizado.git
```

## Configuración y puesta en marcha
Ingresar a la carpeta del proyecto

`cd node-mysql-dockerizado` 

Copiar el archivo .env.example y renombrarlo a .env

`cp .env.example .env`

Modificar las variables de entorno a gusto.

### Levantar ambiente con docker-compose
Si está usando docker-compose, una vez que ya clonó el repositorio.
```
# construir imagen (opcional)
docker-compose build
# up daemon
docker-compose up -d
```
## Variables de entorno
Las variables de entorno de .env se explican a continuación:

- **MYSQL_USER**: usuario de mysql
- **MYSQL_PASSWORD**: contraseña para el usuario
- **MYSQL_ROOT_PASSWORD**: contraseña para root
- **MYSQL_DATABASE**: base de datos para Laravel
- **MYSQL_LOCAL_PORT**: puerto de mysql local
- **MYSQL_DOCKER_PORT**: puerto dentro del contenedor, este va a variar si la base es de prueba