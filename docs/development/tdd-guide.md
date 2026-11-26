# TDD

Por cada comportamiento aprobado:
1. Escribir prueba observable y ejecutarla; RED debe fallar por el comportamiento que falta, no por entorno roto.
2. Conservar comando, resultado y commit de prueba cuando corresponda.
3. Implementar el mínimo cambio y ejecutar la misma prueba: GREEN.
4. Refactorizar solo si aporta y ejecutar regresión.
5. Registrar resultado, commit/PR y estado en tasks.md y matriz.

Unitarias: entidades y casos de uso mediante dobles de puertos. Integración: adaptadores HTTP, seguridad, PostgreSQL real aislado y transacciones. E2E: flujos de roles, catálogo, pedido y confirmación. Incluir concurrencia, rollback y persistencia tras reinicio. No usar datos reales o producción. Pytest es candidato; M01 confirmará herramientas y comandos. Los CSV iniciales son planificación, no evidencia.
