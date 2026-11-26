# Registro de prompts

Estado inicial: no hay interacciones ejecutadas con OpenCode registradas. Los prompts preparados se identifican como propuestos hasta que el operador confirme su ejecución.

El registro se mantiene en la rama chatgpt(docs/audit)-prompt-ledger. No registrar conversaciones triviales, claves de API, JWT reales, credenciales ni datos personales.

Para cada interacción relevante usar [plantilla](audit/prompt-template.md); conservar el texto exacto (redactando únicamente secretos, si existieran), resultado real o enlace a evidencia, modo PLAN/BUILD, modelo si se conoce, módulo, rama, commit/PR y auditoría. Numeración PROMPT-001 en adelante. Las respuestas no recibidas quedan pendientes.
