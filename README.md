## Notas
El docker compose utilizado fue docker-compose.prod.yml
Al cargar el repositorio en VS Code el archivo .env tenia una palabra al final (.env.template) por lo cual al ejecutar el docker compose no lo detectaba ya que el nombre original era .env, se tuvo que renombrar el archivo y una vez hecho eso y despues de ejecutar el comando docker compose up --build los servicios empezaban a descargar sus complementos asi como se asignaban los puertos y las credenciales de MySQL

## Archivo .ENV

## Docker Compose Nodejs MysqL

This is a simple example of a docker-compose file that creates a nodejs and mysql container.

### Considerations

- When mysql container is created, it will create a root user and a another user in the `MYSQLDB_USER` environment variable, each with its own password

### Commands

```sh
docker-compose up # to execute development
docker-compose -f docker-compose.prod.yml up # to execute production
```
