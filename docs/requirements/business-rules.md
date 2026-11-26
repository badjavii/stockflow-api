# Reglas de negocio

Fuente: enunciado §10, pp. 5–6. Formulaciones resumidas; numeración original.

| ID | Regla | Comportamiento | Módulo propuesto |
|---|---|---|---|
| RN-01 | Cantidad válida | No agregar cantidad igual o inferior a cero. | M04 |
| RN-02 | Pedido con productos | No confirmar un pedido vacío. | M05 |
| RN-03 | Disponibilidad de stock | No confirmar si algún producto carece de stock suficiente. | M05 |
| RN-04 | Actualización del inventario | Descontar cantidades tras confirmación correcta. | M05 |
| RN-05 | Confirmación única | No confirmar un pedido ya confirmado. | M05 |
| RN-06 | Cálculo del total | Calcular total a partir de precios y cantidades. | M04; M05 |
| RN-07 | Propiedad del pedido | Cliente solo consulta y modifica pedidos propios. | M04; M05 |
| RN-08 | Autorización administrativa | Administración de productos solo ADMIN. | M02; M03 |
