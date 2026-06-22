# App web modelo v26

Versión basada en v25 cloud.

Cambios:
- Resumen superior ajustado: Total gastos variables muestra cero en meses sin inicializar y valor real en meses inicializados.
- Base usada flujo GV muestra presupuesto solo cuando el mes no está inicializado y cero cuando ya está inicializado, sin nota adicional.
- Las notas generadas por inputs se reconstruyen automáticamente al editar o eliminar inputs.
- Menú lateral organizado por submenús: Gestión meses, Informes, Modelo y respaldo.
- Mantiene compatibilidad con Firebase/Firestore y el modelo guardado en la nube.
