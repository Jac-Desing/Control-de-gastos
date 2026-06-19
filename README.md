# App web modelo v11

Versión basada en la v10 funcional y en la lógica del Excel original.

## Mejora principal

- Encabezados de meses fijos tipo Excel mientras se navega por el cuerpo del modelo.
- La tabla principal ahora tiene desplazamiento interno vertical y horizontal.
- Se conserva la primera columna fija para no perder el concepto.

## Se conserva de la v10

- Tema oscuro.
- Resumen superior.
- Conceptos editables en todas las secciones.
- Meses/columnas dinámicas.
- Nombre de mes editable.
- Comentarios por celda.
- Columna de saldos iniciales editable, ocultable/mostrable.
- Ingresos negativos, gastos positivos.
- Saldos negativos como superávit y positivos como déficit.
- Saldos bancos digitados positivos, tratados como negativos para totales.
- Cuadre de caja según la lógica del modelo.

## Uso

1. Abrir `index.html` en Chrome o Edge.
2. El modelo principal se desplaza dentro de su propio panel.
3. Al bajar por las filas, los títulos de mes quedan visibles arriba del panel.
4. Para conservar cambios, usar el guardado del navegador.


## Versión 12

- Mantiene la lógica y funcionalidades de la versión 11.
- Los campos numéricos editables del cuerpo muestran separadores de miles en formato colombiano.
- Al hacer clic en una celda, el valor se muestra sin formato para facilitar la edición; al salir de la celda vuelve a formatearse automáticamente.

## Cambios v13

- Se eliminó del resumen superior el indicador de **Saldo final bancos**.
- Se conserva el cálculo interno de bancos para el cuadre de caja y el resumen por mes.
- Se mantienen todas las funcionalidades de la v12: formato con separador de miles, encabezados fijos, comentarios por celda, conceptos editables y meses dinámicos.
