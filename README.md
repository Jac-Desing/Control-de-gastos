# App web modelo v38

Versión construida sobre la **v36.2 corregida** suministrada por el usuario.

Incluye estas correcciones:

- Reparación del formulario **Crear concepto**, disponible solo para:
  - Gastos variables.
  - Otros movimientos.
- Submenús laterales desplegables por categoría.
- Cierre de mes con validación previa: el **cuadre de caja debe ser cero**.
- La columna **Saldo inicial bancos** se muestra únicamente en la sección **Saldos bancos** y conserva el botón de ocultar/mostrar.
- Se elimina el drag & drop de conceptos.
- Se agrega campo **Orden** por concepto dentro de cada sección.
- Cada sección tiene botón **Orden / Guardar orden**.
- El orden se guarda de **menor a mayor** y persiste en Firebase.

No se modifica Firebase Auth, Firestore, login ni estructura principal del modelo.
