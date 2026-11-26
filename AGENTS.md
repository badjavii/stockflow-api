# Instrucciones para agentes

StockFlow API, proyecto final de Desarrollo de APIs con Python (UCAB).

## Orden de lectura

1. [Constitución](specs/constitution.md).
2. [Requisitos](docs/requirements/requirements.md), [reglas](docs/requirements/business-rules.md) y [trazabilidad](docs/requirements/traceability.csv).
3. [Memoria](memory.md), [arquitectura](docs/architecture.md) y [módulo asignado](specs/README.md).
4. [SDD](docs/development/sdd-guide.md), [TDD](docs/development/tdd-guide.md), [Git](docs/development/git-workflow.md) y [workflow agéntico](docs/development/agent-workflow.md).

## Contrato operativo

- OpenCode en PLAN analiza y propone; no modifica archivos. Solo en BUILD, tras aprobación humana, materializa documentos o cambios explícitamente autorizados.
- Trabajar una tarea verificable por vez. No implementar sin spec, plan y tasks revisados. No adelantar tareas ni ampliar alcance.
- Dominio y aplicación no importan FastAPI, ORM ni PostgreSQL; los adaptadores dependen de los contratos internos.
- Aplicar RED (fallo por comportamiento esperado), GREEN (mínimo cambio), REFACTOR si procede y regresión. Para cambios documentales no fingir RED/GREEN.
- Entregar comandos exactos, salidas reales resumidas, archivos modificados, decisiones, riesgos y SHA si existe. No declarar éxito sin evidencia.
- Mantener tasks.md y memory.md con estado real; registrar decisiones pendientes. No editar docs/PROMPTS.md ni docs/audit/ sin instrucción humana: los mantiene el auditor.
- Documentación en español; nombres de código y commits en inglés, Python legible, funciones explícitas, sin abstracciones innecesarias.
- No crear credenciales reales, exponer tokens, cambiar permisos, modificar main, fusionar PR, hacer force push ni desplegar sin autorización. No modificar tests para ocultar fallos.
- El equipo humano conserva responsabilidad y aprobación. ChatGPT actúa como segundo PO y auditor, no implementador funcional.
