# App web modelo v23

Versión basada en la v22 cloud estable y compatible con Firestore.

## Cambios v23

1. Las notas generadas desde el formulario de gastos variables ahora se acumulan por viñetas en la celda correspondiente, incluyendo fecha, mes, concepto, acción y valor del input.
2. El informe principal ahora es **Informe gastos variables Excel** y resume los inputs realizados desde el formulario para gastos variables.
3. El antiguo historial de cambios se conserva como informe separado: **Historial cambios Excel**.
4. Las opciones superiores se movieron a un panel lateral izquierdo ocultable mediante botón de tres rayas.
5. Los indicadores superiores ahora muestran:
   - Saldo proyectado del mes actual.
   - Cuadre de caja del mes actual.
   - Saldo proyectado del último mes visible.
   - Cuadre de caja del último mes visible.
6. Se eliminó el indicador de mes más deficitario.

## Compatibilidad

Mantiene la ruta de Firestore:

```text
users/{uid}/models/principal
```

Mantiene el modelo guardado en el campo `data` como JSON serializado, por lo que es compatible con los datos ya creados en la v22.

## Publicación

Subir a GitHub reemplazando:

- `index.html`
- `README.md`

No borrar datos en Firebase.
