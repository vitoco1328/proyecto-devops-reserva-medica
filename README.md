# Proyecto DevOps: reserva médica

Plantilla estática en español para una página de reserva de citas médicas. El formulario es solo visual: no envía ni almacena datos hasta conectarlo a un backend.

## Estructura

```text
src/
  index.html
  styles.css
.github/
  workflows/
    devopsautomation.yml
Dockerfile
docker-compose.yml
.gitignore
.env.example
README.md
```

## Ejecutar localmente

Requiere Docker y Docker Compose.

1. Copia `.env.example` a `.env` si quieres configurar el puerto.
2. Ejecuta `docker compose up --build`.
3. Abre `http://localhost:8080` (o el puerto definido en `APP_PORT`).

El workflow de GitHub Actions construye la imagen Docker en cada push y pull request hacia `main`.
