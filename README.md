# App web modelo v28

Versión cloud basada en v27.

Cambios principales:
- Menú inicial después del login: Ver modelo completo o Agregar inputs.
- En vista móvil se puede abrir solo el formulario de inputs.
- Ppto Gastos Variables se calcula automáticamente desde Gastos variables antes de inicializar el mes.
- Al inicializar el mes, el presupuesto queda fijo, Gastos variables queda en cero y bloqueado.
- Otros movimientos queda editable manualmente solo mientras el mes no esté inicializado; después solo cambia por inputs.
- Se mantiene sincronización Firebase/Firestore y compatibilidad con datos previos.
