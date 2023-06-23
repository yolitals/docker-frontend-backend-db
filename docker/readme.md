# Desplegar la aplicación utilizando docker compose

## Prerrequisitos

- Install docker ([Instalación en Ubuntu](https://docs.docker.com/engine/install/ubuntu/))
- Asegurarse que la computadora o maquina virtual tenga acceso a internet

## Ejecutar los contenedores de la aplicación

```sh
# Clonar este repositorio
$ git clone https://github.com/yolitals/docker-frontend-backend-db.git

## Moverse hacia la carpeta donde se encuentra el archivo docker-compose.yml
$ cd docker-frontend-backend-db/docker

## Crear el directorio donde se montara la base de datos
$ mkdir -p /tmp/data
# Si se utiliza un directorio diferente se tendrá que actualizar el argumento: device, en la sección: volumes del archivo docker/docker-compose.yml

## Agregar usuario actual al grupo de docker
$ sudo gpasswd -a $USER docker
## Es necesario reiniciar la sesión para que los cambios se apliquen

## Install docker-compose if is not installed
sudo apt  install docker-compose

## En el archivo docker/docker-compose.yml actualizar el endpoint de la variable REACT_APP_API_URL, utilizar la IP publica del host.

## Crear una regla de firewall que permita trafico de ingreso al puerto 3001, que es donde estará corriendo el backend.

## Ejecutar los contenedores
$ docker-compose up -d

```
