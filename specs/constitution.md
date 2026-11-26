# Constitución de trabajo

1. Alcance: backend REST FastAPI, PostgreSQL, OAuth2/JWT, UUID, Docker Compose; perfiles ADMIN/CUSTOMER. Respetar enunciado y RN-01 a RN-08. No frontend ni ampliaciones no aprobadas.
2. SDD: necesidad → especificación → plan → tareas → pruebas → implementación → verificación. Cada módulo mantiene spec.md, plan.md y tasks.md. Los criterios se aprueban antes de programar.
3. TDD: prueba primero, RED real, implementación mínima, GREEN, refactor si aporta y regresión. Conservar evidencia temporal y commits identificables. No contabilizar pruebas planificadas como ejecutadas.
4. Arquitectura: dominio independiente de FastAPI y PostgreSQL; casos de uso coordinan puertos. Adaptadores e infraestructura resuelven tecnología. Las restricciones de persistencia complementan, no sustituyen, reglas de dominio.
5. Seguridad: contraseñas con hash seguro, autorización por perfil y propiedad, secretos fuera de Git, JWT validado y configuración explícita. No confiar en identidad o perfil proporcionados por el cliente.
6. Integridad: UUID, importes sin pérdida de precisión, confirmación y descuento atómicos; verificar concurrencia y rollback. Las decisiones de diseño requieren aprobación.
7. Revisión humana: PLAN antes de BUILD; equipo aprueba contratos y PR. ChatGPT audita y dirige prompts; OpenCode implementa.
8. Evidencia: mantener trazabilidad requisito → criterio → tarea → prueba → resultado → commit/PR; distinguir propuesta, aprobación y ejecución. PROMPTS.md registra interacciones relevantes reales.
9. Git: ramas desde develop, PR a develop, main solo release. No reescribir historial ni mezclar cambios ajenos. Conservar ramas como evidencia.
10. Terminado: criterios cubiertos, regresión ejecutada, revisión de diff y seguridad, tasks/memory actualizados, evidencia y aprobación humana. Documentación sin duplicaciones innecesarias.
