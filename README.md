Practica: Despliegue de WordPress con Docker Compose y Jenkins
Objetivo

El objetivo de esta practica fue crear un ambiente de WordPress utilizando Docker Compose, almacenar el proyecto en GitHub y automatizar el despliegue mediante un Pipeline en Jenkins.

Archivos del proyecto
docker-compose.yml
.env
Jenkinsfile
README.md
Pasos realizados
Se configuró un archivo docker-compose.yml con los servicios de WordPress y MySQL.
Se creó un archivo .env para almacenar las variables de configuración.
Se levantó el ambiente utilizando Docker Compose.
Se verificó que los contenedores, la red y los volumenes se crearan correctamente.
Se subió el proyecto a un repositorio en GitHub.
Se creó un Pipeline en Jenkins para automatizar el despliegue del proyecto.
Ejecución

Para iniciar el ambiente se utilizó el siguiente comando:

docker compose up -d


Se comprobó que los contenedores estuvieran en ejecución con:

docker ps

Tambien se verificó la creación de la red y los volumenes con:

docker network ls
docker volume ls

Al finalizar la practica se pudo acceder a WordPress desde el navegador mediante la dirección:

http://localhost:8080

Mostrando correctamente el asistente de instalación de WordPress.