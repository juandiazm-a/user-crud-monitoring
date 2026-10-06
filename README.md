User CRUD Monitoring

Proyecto para gestionar usuarios y revisar el funcionamiento de una API.

¿Qué usamos?
FastAPI: para crear la API.
PostgreSQL: para guardar los usuarios.
Docker: para ejecutar los servicios.
Docker Compose: para iniciar todos los servicios.
Prometheus: para revisar las métricas de la API.
Grafana: para mostrar las métricas en un dashboard.

¿Qué hace?

La API permite:

Crear usuarios.
Consultar usuarios.
Mostrar métricas de la API.

También tenemos métricas de:

Usuarios creados.
Uso de CPU.
Memoria utilizada.

Servicios

FastAPI: `http://localhost:8000`
Prometheus: `http://localhost:9090`
Grafana: `http://localhost:3000`
PostgreSQL: puerto `5432`

Ejecutar el proyecto

Desde la carpeta del proyecto:

```bash
docker compose up --build
```

Para revisar los contenedores:

```bash
docker compose ps
```

## Estructura

```text
user-crud-monitoring/
├── app/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   └── Dockerfile
├── prometheus/
│   └── prometheus.yml
├── docker-compose.yml
└── README.md
```

Este proyecto integra una API, una base de datos y herramientas para revisar su funcionamiento.
