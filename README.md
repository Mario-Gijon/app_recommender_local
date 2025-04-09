
# Recommender Local App

Aplicación de recomendación de películas. Desarrollado con React y FastAPI, desplegado con Docker Compose.
## Requisitos
- Docker
- Docker Compose

## Instalación
1. Clona este repositorio:
   ```bash
   git clone https://github.com/mariogijon/app-recommender.git
   cd app-recommender

2. Descarga y ejecuta los contenedores con docker-compose:
   ```bash
   docker-compose pull
   docker-compose up

## Configuración en local
Para actualizar la lista de películas, es necesario modificar la variable de entorno del fichero docker-compose.yml.

- Actualizar lista de películas (necesita acceso a internet):
   
   MOVIES_SOURCE: "api"

- Ejecutar con la información local
   
   MOVIES_SOURCE: "local"

## Acceder a  la app

- Url: http://localhost:5173

- Documentación de la api: http://localhost:8000/docs

## Importante
La app descargará la información de películas en un directorio data/, donde se encuentra las imágenes y un fichero csv con la información de cada película. En caso de no encontrarse la carpeta, el servidor creará y actualizará la lista de películas.

