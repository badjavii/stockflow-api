# Workflow agéntico

El equipo humano es PO principal y primer revisor; ChatGPT es segundo PO/auditor y gestor de estructura, prompts y revisión; OpenCode es agente desarrollador; FreeLLM API es proveedor local de modelos. No es dependencia del backend entregable.

1. ChatGPT prepara un prompt con fuente, módulo, alcance y salida esperada; humano lo ejecuta en PLAN.
2. OpenCode devuelve propuesta sin cambios. Humano comparte respuesta real y decide con auditor.
3. En BUILD se autoriza exclusivamente materializar spec/plan/tasks aprobados, y luego una tarea de pruebas RED o implementación GREEN por instrucción explícita.
4. Humano comparte salida, comandos, diffs y commits (sin secretos). Auditor verifica contra GitHub y devuelve aprobación, observaciones o prompt correctivo.
5. PR a develop y aprobación humana. Actualizar tareas, memoria y trazabilidad. El auditor registra prompt exacto, modo, modelo si conocido, respuesta real, commit y resultado en su rama.

No ejecutar un prompt global para generar toda la API. No afirmar que un prompt fue enviado antes de recibir evidencia. No usar la rama de auditoría para implementación. Si se desconoce modelo o resultado, indicar pendiente/no informado.
