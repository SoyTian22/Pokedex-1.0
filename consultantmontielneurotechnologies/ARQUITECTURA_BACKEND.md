# Arquitectura backend

## Componentes

1. API REST: operaciones rápidas y endpoints claros.
2. PostgreSQL + pgvector: datos relacionales y búsqueda semántica.
3. Redis: cache, colas y coordinación de eventos.
4. RAG legal: ingesta normativa, embeddings y recuperación de fragmentos.
5. Identidad digital responsable: validación reforzada, roles y trazabilidad.
6. IoT: sensores de flota, caminería, ambiente y logística.
7. Observabilidad: logs, auditoría y métricas.

## Endpoints principales

- GET /api/health
- GET /api/departments
- GET /api/solutions
- POST /api/diagnostic
- GET /api/cases
- POST /api/identity/verify
- GET /api/iot/telemetry
- GET /api/legal/rag-demo

## Comentarios Cristian: ejemplo técnico

Un carrusel de expedientes no debe cargar todos los expedientes en pantalla. El backend prioriza por urgencia, vencimiento y necesidad de firma. El frontend consume nodos paginados y mantiene la interfaz fluida.