# Análisis de Validación y Modelado

## Validación:  ¿Por qué es preferible implementar la validación de datos a nivel de Base de Datos (con JSON Schema) en lugar de hacerlo únicamente en el código de la aplicación (backend)?
Implementar validación a nivel de base de datos con JSON Schema garantiza la integridad de los datos incluso si el backend falla o se omite. Esto evita que ingresen documentos inválidos desde cualquier cliente o script, fortaleciendo la consistencia del sistema.

## Relación 1 a 1:  Explicar la ficha_veterinaria como una relación 1-a-1 embebida. ¿Por qué fue un buen enfoque? ¿Bajo qué circunstancias es mejor modelarla como referenciada (en su propia colección)?
Se embebió la ficha veterinaria dentro de la criatura porque es un dato que pertenece exclusivamente a ella y siempre se consulta junto al documento principal. Si la ficha tuviera múltiples actualizaciones históricas o un manejo independiente por veterinarios, sería mejor referenciarla.

## Relación 1 a N (Inventario y Criaturas)
- **Inventario (embebida)**: se eligió embebida porque los ítems del guardián solo tienen sentido dentro de su documento.
- **Criaturas (referenciada)**: se usó referenciada para evitar duplicar datos del guardián y permitir que una criatura mantenga un vínculo estable incluso si el guardián cambia o se elimina.

Este modelo combina eficiencia de consulta con control de integridad, balanceando redundancia y escalabilidad.
