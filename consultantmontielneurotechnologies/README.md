# Consultant Montiel Neurotechnologies - GovTech Lab

Proyecto fullstack preparado para Montiel Labs International Technologies and Solutions.

## Contenido entregado

- Frontend editorial black con smoke transitions, mapa interactivo, cuestionarios, gráficos y módulos clickeables.
- Backend FastAPI con endpoints REST.
- API para departamentos, soluciones, diagnóstico, expedientes, identidad digital responsable, IoT y RAG legal demostrativo.
- PostgreSQL + pgvector con schema inicial.
- Redis preparado para cache/colas.
- Nginx para servir frontend y proxyear API.
- Docker Compose para ejecución local.
- Configuración Netlify para frontend.
- Terraform/Ansible base para cloud/IaC.
- GitHub Actions CI.

## Ejecutar

```bash
cd consultantmontielneurotechnologies
docker compose up --build
```

Frontend: http://localhost:8080
API: http://localhost:8000/docs

## Comentario para Daniel

Daniel, esta demo no busca vender una pantalla. Busca mostrar cómo una Intendencia puede convertirse en un sistema operativo institucional: procesos, personas, evidencia, ciudadanía, normativa, comunicación y decisiones en una misma arquitectura. La propuesta empieza con diagnóstico, sigue con piloto y termina en gobierno medible.

## Nota de publicación

El paquete completo está preparado como ZIP descargable y puede subirse como repositorio dedicado para Netlify, Vercel o un despliegue Docker fullstack.