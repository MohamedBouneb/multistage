# Docker multi-stage : React (Vite) + Django

Dockerfiles utilisés dans mon PFE chez DM Nova (FormTemple).

## Frontend (React/Vite → Nginx)
- Stage 1 : build avec node:20-alpine
- Stage 2 : image finale nginx:alpine avec uniquement les fichiers statiques


## Backend (Django + uv + Gunicorn)


## Points clés
- Builds reproductibles (`--frozen-lockfile`, `uv sync --frozen`)
- Cache Docker optimisé
- Image frontend minimale

## Stack complète du projet
Docker Compose, PostgreSQL, Redis, Celery, Nginx, GitHub Actions → Azure, Prometheus/Grafana
