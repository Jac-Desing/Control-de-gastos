# App web modelo v32

Versión basada en v31 con mejoras de estados e inputs.

## Cambios v32

- Estados de mes concentrados en el formulario de inputs y en el control de presupuesto:
  - Sin inicializar
  - Inicializado
  - Abierto
  - Cerrado
- Se eliminan estados visuales de otros puntos del informe.
- Entrada directa al formulario: solo acción **Sumar**.
- Edición desde Inputs registrados: cierra automáticamente el cuadro, abre el formulario, fuerza acción **Reemplazar** y exige guardar o cancelar antes de continuar.
- El reemplazo de un input modifica ese input sin destruir otros inputs del mismo concepto/mes.

Subir a GitHub reemplazando `index.html` y `README.md`.
