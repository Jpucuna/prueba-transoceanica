# Prueba Transoceanica

Este proyecto se configura y ejecuta fácilmente utilizando **Docker**. Asegúrate de tener Docker y Docker Compose instalados en tu máquina para comenzar.

## Requisitos

- **Docker**: [Instalar Docker](https://docs.docker.com/get-docker/)
- **Docker Compose**: [Instalar Docker Compose](https://docs.docker.com/compose/install/)

## 🛠 Tecnologías Utilizadas

Este proyecto fue desarrollado utilizando las siguientes tecnologías:

- **Next.js** – Framework de React para el frontend.
- **NestJS** – Framework para construir aplicaciones backend escalables con Node.js.
- **PostgreSQL** – Base de datos relacional utilizada para almacenar los feriados.
- **Docker** – Contenedores para facilitar la ejecución y despliegue del entorno completo.

## 📅 Gestión de Feriados

El aplicativo permite gestionar diferentes tipos de feriados en Ecuador:

- **Feriados Nacionales**: Fechas oficiales a nivel nacional.
- **Feriados Locales**: Celebraciones regionales o cantonales.
- **Feriados Personales**: Fechas personalizadas por cada usuario.

> ⚠️ Solo los **feriados personales** pueden ser **editados o eliminados**.  
> Esto garantiza que los feriados **nacionales y locales** más comunes no puedan ser manipulados, manteniendo la integridad del calendario oficial.

## Configuración del entorno

1. Clona este repositorio en tu máquina local:

   ```bash
   git clone --recurse-submodules <Link del repo>
   cd prueba-transoceanica

2. Crea el archivo .env a partir del archivo env.example:
    ```bash
    En la ruta del backend calendar-backend\env.example tendras el archivo que deberas modificar.
  Importante: No modifiques los valores ya puestos en el archivo .env. Este archivo contiene configuraciones por defecto necesarias para el correcto funcionamiento de la aplicación. 🙂

## Levanta el proyecto con Docker y comprueba el funcionamiento del aplicativo.
   Una vez que hayas configurado el archivo .env, puedes levantar los contenedores usando Docker Compose, esto se realizara fuera de las carpetas frontend y backend, el comando debe ser ejecutado en la carpeta principal (prueba-transoceanica). Esto descargará las            imágenes necesarias y configurará el entorno de manera automática.

   Deseo resaltar ademas que el aplicativo esta configurado para lanzarse desde localhost:3000 🚀
  ```bash
      docker-compose up --build

  
