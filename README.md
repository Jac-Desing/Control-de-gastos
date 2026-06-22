# App web modelo v30

Versión basada en la v29 cloud/Firebase.

Cambios principales:

- La opción **Reemplazar** solo aparece cuando se edita un input existente.
- Al editar un input desde **Inputs registrados**, se cierra la ventana, se abre el formulario, se fuerza modo reemplazar y se exige guardar o cancelar antes de hacer otra acción.
- Las secciones del modelo se pueden expandir o contraer desde el botón junto al nombre de cada sección.
- El resumen por mes se puede contraer. En vista contraída muestra solo: saldo proyectado, total bancos y cuadre de caja.
- Nuevo formulario para crear conceptos en **Gastos variables** y **Otros movimientos**.
- El formulario de inputs ya no aparece siempre en el informe completo; se abre desde un botón como cuadro de diálogo.
- Conserva Firebase, Firestore, autenticación y la estructura de datos en nube.

Para actualizar GitHub Pages, reemplaza `index.html` y `README.md` en el repositorio.
