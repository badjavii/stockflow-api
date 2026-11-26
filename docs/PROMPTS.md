# Registro de prompts

Estado inicial: no hay interacciones ejecutadas con OpenCode registradas. Los prompts preparados se identifican como propuestos hasta que el operador confirme su ejecución.

El registro se mantiene en la rama chatgpt(docs/audit)-prompt-ledger. No registrar conversaciones triviales, claves de API, JWT reales, credenciales ni datos personales.

Para cada interacción relevante usar [plantilla](audit/prompt-template.md); conservar el texto exacto (redactando únicamente secretos, si existieran), resultado real o enlace a evidencia, modo PLAN/BUILD, modelo si se conoce, módulo, rama, commit/PR y auditoría. Numeración PROMPT-001 en adelante. Las respuestas no recibidas quedan pendientes.


## PROMPT-001 : Análisis y especificación de Foundation

- Estado: propuesto; no enviado ni ejecutado.
- Fecha de preparación: 2026-11-26.
- Modo previsto: PLAN.
- Modelo y operador: pendientes.
- Módulo: M01.
- Rama prevista: opencode(feat/infra)-foundation.
- Prerrequisito: PR de inicialización integrado y rama de trabajo creada desde develop actualizado.

### Prompt exacto propuesto

```text
Actúa como agente desarrollador de StockFlow API en modo PLAN. No modifiques archivos ni generes código todavía.

Lee AGENTS.md, memory.md, specs/constitution.md, specs/README.md, specs/templates/, docs/architecture.md, docs/requirements/ y docs/development/. Consulta el enunciado original local si está disponible y señala cualquier discrepancia o dato faltante.

Trabaja exclusivamente el módulo M01 Foundation (RF-01, RF-02, RF-03, RF-04 y aspectos de RF-15). Propón el contenido de spec.md, plan.md y tasks.md, con criterios de aceptación identificables, estrategia RED/GREEN para comportamientos verificables, dependencias y decisiones pendientes. Justifica una estructura hexagonal mínima, versión de Python, opciones de persistencia/migraciones, configuración, Docker Compose y estrategia de pruebas aisladas. No incorpores autenticación, productos ni pedidos funcionales. No impongas una biblioteca o decisión no aprobada. Identifica riesgos y preguntas que bloqueen el inicio.

Devuelve la propuesta y un resumen de decisiones para revisión humana. No edites archivos, no hagas commits, no ejecutes instalaciones ni avances a BUILD.
```

### Resultado real

Pendiente de ejecución.

### Auditoría

Pendiente de respuesta de OpenCode y revisión humana.
