# App web modelo v24

Versión basada en la v23 cloud y compatible con los datos ya guardados en Firebase.

## Cambios v24

- Los inputs del formulario quedan registrados como entradas activas con ID propio.
- Los inputs activos se pueden consultar, editar y eliminar desde la app.
- Al eliminar un input, se retira del modelo y deja de aparecer en el informe de inputs.
- El formulario permite registrar inputs en:
  - Gastos variables
  - Otros movimientos
- El informe de inputs Excel se basa en los inputs activos del formulario, no en el historial general de cambios.
- El historial de cambios se conserva como informe separado.
- Se puede ajustar el ancho de columnas:
  - arrastrando el borde derecho de los encabezados
  - o desde el panel lateral con la opción Ajustar ancho columnas

## Nube

Mantiene la misma ruta de Firestore:

users/{uid}/models/principal

El modelo continúa guardándose como JSON serializado en el campo `data`, por lo que conserva compatibilidad con v22 y v23.
