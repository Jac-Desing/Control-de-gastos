# App web modelo v25

Versión basada en la v24 cloud, compatible con el modelo guardado en Firebase.

Cambios principales:
- Vista de inputs registrados en ventana/modal consultable desde el menú lateral.
- Inicialización independiente por mes para Gastos variables.
- Nueva sección Presupuestos Gastos variables con la línea Ppto Gastos Variables.
- Al inicializar un mes, el presupuesto se toma del total existente de Gastos variables, luego esos valores quedan en cero y bloqueados para edición manual.
- Para meses sin inicializar, el flujo usa el presupuesto de gastos variables; para meses inicializados, usa el total real de gastos variables.
- Resumen adicional por mes: presupuesto, gasto real y diferencia.
- Mantiene inputs editables/eliminables, Otros movimientos en formulario, ajustes de ancho de columnas, Firebase/Firestore y compatibilidad con datos existentes.
