# App web modelo v31

Versión basada en la v30 cloud/Firebase.

Cambios principales:

- Reorganización responsive del formulario para PC y móvil.
- Fusión de conceptos en Gastos variables y Otros movimientos.
- Botón de inicialización de mes desde el formulario.
- Cierre de mes con validación de fecha calendario, bloqueo de edición e inputs, y respaldo independiente.
- Apertura de mes cerrado con advertencia.
- Estados visuales: abierto, inicializado y cerrado.

Se mantiene la ruta cloud `users/{uid}/models/principal` y el campo `data` serializado como JSON.
