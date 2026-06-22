# App web modelo v29

Versión basada en la v28 cloud/Firebase.

## Cambio principal

- No permite registrar inputs en meses no inicializados.
- Si se intenta ingresar un input en un mes no inicializado, la app muestra un error y bloquea el botón de aplicación.
- La validación se ejecuta al seleccionar mes y nuevamente al guardar.

## Regla operativa

- Mes sin inicializar: edición manual permitida en Gastos variables / Otros movimientos, pero inputs bloqueados.
- Mes inicializado: edición manual bloqueada en Gastos variables / Otros movimientos, inputs permitidos.

## Publicación

Subir a GitHub Pages reemplazando `index.html` y `README.md`.
