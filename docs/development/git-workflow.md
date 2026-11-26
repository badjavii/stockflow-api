# Flujo Git : StockFlow API

main: entrega estable y etiquetas; develop: integración; ramas individuales desde origin/develop. PR a develop, revisión humana, auditoría y CI cuando exista; PR develop → main para entrega. Conservar ramas y commits RED/GREEN; preferir merge commit para preservar el historial. No borrar ramas ni force push.

Convención: `<author>(<kind>/<layer>)-<short-description>`. Autor identifica el responsable humano o agente asistente (el responsable humano se registra aparte). kind: docs, feat, test, fix, chore, ci, refactor. layer: spec, audit, infra, domain, application, adapters, auth. Inglés, guiones, sin dos puntos.

```bash
git fetch origin
git switch develop
git pull --ff-only origin develop
git switch -c 'opencode(feat/infra)-foundation'
git push -u origin 'opencode(feat/infra)-foundation'
```

Commits: docs: define foundation specification; test: define behavior; feat: implement behavior; refactor: simplify. PR incluye requisitos, criterios, evidencias RED/GREEN y regresión, auditoría, riesgos, secretos y alcance. No fusionar sin aprobación.

Rama de auditoría: chatgpt(docs/audit)-prompt-ledger. Solo modifica docs/PROMPTS.md y docs/audit/; sincronizar desde develop mediante merge sin reescribir historial. Integrar evidencia por PR antes de entrega. Mantener docs/project/branch-ledger.csv en ramas documentales o PR correspondiente; evitar cambios simultáneos al mismo registro.

A diferencia de RutasVenezuela, no se reemplaza README.md por un README temporal de rama: la trazabilidad vive en el registro y PR, evitando conflictos con el README institucional.
