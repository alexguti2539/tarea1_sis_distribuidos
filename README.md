# Tarea 1: Sistema de Caché Distribuido para Logística Urbana

Este proyecto implementa un sistema distribuido diseñado para optimizar consultas geoespaciales sobre edificaciones en el área metropolitana de Santiago. Utiliza una arquitectura basada en contenedores con **Docker**, una capa de caché en memoria con **Redis** y procesamiento de datos vectorizado con **Python (Pandas)**.

## Requisitos Previos

Para ejecutar este sistema, es necesario tener instalado:
* [Docker Desktop]
* [Docker Compose]

## Estructura del Proyecto

* `app.py`: Aplicación principal que contiene el Generador de Tráfico, el Generador de Respuestas y el Almacenamiento de Métricas.
* `docker-compose.yml`: Orquestador de los servicios (Aplicación + Redis).
* `Dockerfile`: Configuración de la imagen de Python y dependencias.
* `datos/`: Carpeta que contiene el dataset `santiago_zonas_limpio.csv`.

## Instrucciones de Despliegue y Ejecución

Siga estos pasos para ejecutar el sistema y las pruebas de rendimiento:

1. **Clonar o descargar el repositorio:**
   Asegúrese de que todos los archivos estén en la misma carpeta.

2. **Levantar el sistema:**
   Abra una terminal en la ruta del proyecto y ejecute el siguiente comando:
   ```bash
   docker compose up --build
