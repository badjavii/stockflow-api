# Requisitos derivados del enunciado

Identificadores RF asignados por el equipo para trazabilidad; no son códigos originales del docente. Las reglas RN conservan su numeración original.

| ID | Necesidad | Fuente |
|---|---|---|
| RF-01 | API REST FastAPI, exclusivamente backend, validación, errores, dependencias | §§1,13,27 |
| RF-02 | Arquitectura hexagonal y núcleo independiente de tecnología | §14 |
| RF-03 | PostgreSQL persistente, PK/FK UUID en usuarios, productos, pedidos e ítems | §§7,12 |
| RF-04 | Docker Compose con API y PostgreSQL, datos persistentes y documentación | §§12,22,23 |
| RF-05 | Registro público exclusivamente CUSTOMER | §5.1 |
| RF-06 | ADMIN inicial desde entorno, hash seguro e inicialización idempotente | §5.2 |
| RF-07 | OAuth2/JWT, token por credenciales, validar identidad, perfil y validez | §11 |
| RF-08 | Autorización ADMIN/CUSTOMER y rechazo de operaciones no permitidas | §6 |
| RF-09 | ADMIN crea productos: UUID, nombre, descripción opcional, precio, cantidad | §8 |
| RF-10 | Usuarios autenticados consultan catálogo/producto y disponibilidad conforme permisos | §§6,8 |
| RF-11 | CUSTOMER crea pedido propio con UUID, cliente, fecha, estado, ítems y total | §9 |
| RF-12 | CUSTOMER agrega productos y cantidades a pedidos propios | §§6,9 |
| RF-13 | CUSTOMER consulta pedidos propios; ADMIN consulta pedidos del sistema | §§6,9 |
| RF-14 | CUSTOMER confirma pedido propio cumpliendo reglas de stock y confirmación | §§9,10 |
| RF-15 | SDD, TDD, prompts relevantes, memoria, Git, documentación, pruebas y entrega | §§15–26 |

Rutas sugeridas por el docente: POST /auth/register, POST /auth/token, POST /products, GET /products, GET /products/{id}, POST /orders, GET /orders/{id}, POST /orders/{id}/items, POST /orders/{id}/confirm. La consulta de pedidos en colección debe cubrir ambos perfiles según permisos. Los contratos HTTP detallados se aprobarán por módulo.

Fuera de alcance obligatorio: frontend, móvil, GUI, cloud, pagos, facturación, envíos, recuperación de contraseñas, verificación de correo y administración completa de usuarios.

Entrega: URL GitHub antes del miércoles 16/12/2026 11:59 p. m.; equipo 2–3; 15% de asignatura, 60% entrega/40% defensa individual. Todos deben conocer la solución.
