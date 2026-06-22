# App web modelo v27

Versión basada en la v26 cloud.

Ajustes aplicados:
- En el resumen superior, **Ppto gastos variables** solo muestra valor y afecta el flujo cuando el mes no está inicializado.
- En el resumen superior, **Total gastos variables** solo muestra valor y afecta el flujo cuando el mes ya está inicializado.
- Los dos campos son excluyentes por mes.
- Se mantiene el cálculo interno del flujo: presupuesto antes de inicializar y gasto real después de inicializar.
- Se agrega botón directo **Ver inputs registrados** desde el formulario de inputs.
- Se conserva compatibilidad con Firebase/Firestore v22+ usando `users/{uid}/models/principal` y campo `data` serializado como JSON.

Para actualizar GitHub Pages, sube `index.html` y `README.md` reemplazando los existentes.
